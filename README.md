# SUPERSEEDED BY iterate-with-delay

> USE THIS MODULE INSTEAD: https://www.npmjs.com/package/iterate-with-delay

Loop over array but with time delay 

<img alt='' src='https://travis-ci.org/coderofsalvation/delay-for-array.svg'/>

## Usage

    npm install delay-for-array

## Features

* iterates over array but pauses inbetween
* uses callback for each element
* calls extra callback when done

## Example

    delayarr = require('delay-for-array')

    arr = ["one","two","three"];

    delayarr.each( arr, { time:1000 }, function(el,k){

      console.log( new Date()+"element received: "+k+" -> "+el );

    },function(num){

      console.log("finished processing "+num+" items");

    });


