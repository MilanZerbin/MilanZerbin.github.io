+++
title = 'Programming Project'
subtitle = 'Leon Ulbrich'
date = 2026-03-15T08:00:00+02:00
draft = false
tags = ['mentor', 'progprojs']
+++

At Univerity of Augsburg, every Masters-student in Mathematics must spend some time working on a programming project. Its goal is, that "the Student learns the tools to approach a mathematical problem with the help of a computer".

Kai Cieliebak and I have started to host a project on [the Universities High Performance Computing Cluster](https://www.uni-augsburg.de/en/fakultaet/med/profs/exposure-science/aktuelles/linux-compute-cluster-augsburg/) to offer the students the option to pursue such a programming project mentored by us.

Usually, the projects center around combinatorial geometry problems, with the hope of extending the known literature by a couple of cases.

This Project is one of the [programming projects we hosted so far](tags/progprojs)

## No three in line

The *no three in line* problem asks the following question: 
Given a a square of n times n points with integer coordinates in the plane, what is the maximal number f(n) of points one can choose in the square, such that no three of the chosen points are collinear.

By an elementary pidgeonhole-principle-argument, f(n) is at most 2n.

For large n, it has been [suggested by a stochastic argument in 1968](https://doi.org/10.4153%2FCMB-1968-062-3) that it will be impossible to choose 2n such points on an n by n square.

For small n up to 65, configurations with f(n)=2n have been found and are known (see [here for an overview](https://wwwhomes.uni-bielefeld.de/achim/no3in/readme.html))

## The Project

Previous approaches at the problem seem to utilize a classical search tree algorigthm with clever heuristics.
Leon Ulbrichs approach is different. We rewrite the problem into a large instance of a binary linear optimization problem, and wish to use highly parallelizable solvers to push for bigger results than n=65.

