---
Post:
Title:  "quote machine"
Date:   2018-02-16
Categories:

# Creating a Random Quote Machine 

## induction 

I was required to create a random quote machine on FreeCodeCamp .

## instructions 

The program had to have a button , a button that could be clicked and a random 
quote appears on the webpage . It also had to have a tweet button by which you could tweet a quote that you 
have seen on screen and i had to use a API. 

## solution 



$(document).ready(function () {
            function getQuote() {
                $.ajax({
                    type: "GET",
                    url: "https://api.forismatic.com/api/1.0/",
                    jsonp: "jsonp",
                    dataType: "jsonp",
                    data: {
                        method: "getQuote",
                        lang: "en",
                        format: "jsonp"
                    },
                    success: function (quote) {
                        $('q').html(' ' + quote.quoteText + '  ')
                        $('p').html("-" + quote.quoteAuthor)
                        console.log(quote);
                    }

                });

            }
            $('#button').click(function () {
                return getQuote();
            })
        })


It was something new to me because i had to work with API , something that i haven't done before 
so it was a bit challenging . First step was understanding the concept of API so i did some research and cam across 
the definition .Stands for Application Programming Interface. An API is a set of commands, functions, protocols, 
and objects that programmers can use to create software or interact with an external system.
 It provides developers with standard commands for performing common operations so 
 they do not have to write the code from scratch. and this definition i read it up on TechTerms.com
it gave me a better understanding of the concept of API. 

  

So i used ajax to request data from an external source and the source is the one that generated Random quotes.
I returned the results to the webpage. 

## conclusion 

I had fun with this project and learned a lot. 




