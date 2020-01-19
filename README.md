# TOPSIS

#### Abhishek Arora
#### Roll No. 101703021
#### Group - COE 1
#### Project - 1 UCS633
#### TIET

TOPSIS method for multiple-criteria decision making (MCDM)

## Description

The Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS) is a multiple-criteria decision making (MCDM) method.

## Usage

topsis(data, weights, impacts)

## Arguments

data:			A numeric 2D list with m rows for m alternatives and n columns for n criterions.

weights:		A string with numeric values of length equal to number of columns in decision matrix for weights of 	criterions, separated by commas.

impacts:		A string of "+" and "-" signs separated by commas for the way that each criterion influences on the alternatives.

## Output:

A dictionary with key and value pairs.

Key : row_no :	Row number of alternatives in decision matrix.

### Value is list having two elements:
	
	Score: 	TOPSIS score of alternatives.
	Rank:	Rank of alternatives based on TOPSIS scores.

### Examples

  import topsis as tp
  
  tp.topsis(data,'1,1,1,1','+,+,+,+')
