+++
title = "fifawc - CLI app to track FIFA World Cup 2018"
date = "2019-02-10T21:07:55+05:30"
categories = ["blog", "code", "Go(Golang)", "CLI"]
keywords = ["Go(Golang)", "CLI"]
description = "fifawc is a CLI app written in Go to help developers keep track of the ongoing FIFA World Cup 2018 without leaving their terminals. The app uses football-data.org API to provide data."
+++

# fifawc
A small CLI app to track FIFA World Cup 2018.

## About
`fifawc` is a CLI app written in Go to help developers keep track of the ongoing FIFA World Cup 2018 without leaving their terminals. 
The app uses [football-data.org](https://www.football-data.org/) API to provide data.

## Installation
Pre-requisite
- Install Go
- Set PATH variable

Get and Install fifawc app with the command:
> go get -u github.com/nishchayp/fifawc

To run fifawc app from across the system copy fifawc binary to directory pointed by PATH environmental variable.\
Example:
> cp  $GOPATH/bin/fifawc /usr/local/go/bin/

Refer to [this](https://unix.stackexchange.com/questions/18304/how-to-run-my-own-program-without-specifying-its-path) question for more details.

## Usage
```
Usage fifawc [options]Options:
  -f, --fixtures
    	Get fixtures
  -m, --matchday int
    	Filter fixtures by matchday (default -1)
  -s, --squad string
    	Get squad by team name
```

- Get the complete squad of the desired nation
  > fifawc -s [nation]
- Get all fixtures of FIFA World Cup 2018
  > fifawc -f
- Get fixtures filtered by matchday
  > fifawc -f -m [matchday number]
  
  or simply
  > fifawc -m [matchday number]

