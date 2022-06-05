# A Mathematical Approach to Minecraft (MC) Redstone Circuit Design

## Introduction
This document shall serve as a way to study redstone circuits in MC, using mathematical principles. 
It is not meant to serve as an exhaustive guideline. 
In fact, it is encouraged to add upon its knowledge, as long as it is cited in whatever work/project you choose to pursue/make, in whatever format you like.

## Relevant Axioms
Any new field of mathematics requires axioms to be established. 
While a total revamp is not necessary to apply the math to Redstone circuits (and would be quite conceited), 
some new axioms will be introduced that are MC-specific, in order for the math to fit more easily.

As one may have guessed, the axioms are based off of Minecraft's de-obfuscated source-code copy, and other general knowledge already available.

1. MC time proceeds in ticks. By default, there are 20 ticks in 1 real-time second
2. Any MC block has real-life dimensions of 1m by 1m by 1m
3. A redstone signal is able to travel for a distance of 15 blocks before it dies out
4. All redstone-related items take up 1 block each
5. A signal from a redstone source is capable of reaching 15 blocks before it dies out

## Basic Circuitry
Now that the axioms have been introduced, it's time to apply them (and subsequent derivations) to redstone circuits.

The first thing that we'll do is derive a formula for the minimum number of redstone sources required to extend a signal for N blocks.

(Eqn 1)

This equation can also be used for more parallel circuits, all that is needed is to count the total number of blocks for each circuit path, add them all up and apply the same equation (or do each one individually). 

The next circuit that we will study is one which has a repeating (perpetual) signal, a very common setup found in most servers.
