# X-Diff	

Version 0.9.6

X-Diff is a tool for detecting difference between two XML documents.

## Documentation

The core algorithm of X-Diff is described in the paper, "X-Diff: An Efficient Change Detection Algorithm for XML Documents", ICDE 2003.

http://www.cs.wisc.edu/~yuanwang/research/xdiff.pdf

## Installation

Required: Xerces C++ v1.4.0, g++ v2.9.\*

    $ make

for a quick test
   
    $ test.sh

## Running X-Diff

    $ xdiff [-o|-g] [-p percent] xml_file1 xml_file2 result_file

Options:

The default mode is "-o -p 0.3".

  `-o` The optimal mode, to get the diff result with minimum editing
  distance.

  `-g` The greedy mode, to get a diff result quickly, the result may not
  be "optimal".

  `-p` The maximum change percentage allowed. X-Diff will not try to match nodes that are much different from each other.

## Java version

There is a java implementation

http://github.com/albfan/x-diff

## Bug Reporting

Please report any bugs or send your comments to Yuan Wang at yuanwang@cs.wisc.edu

