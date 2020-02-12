# Importent this text don't got Corrected at present and is in DRAFT State don't Judge me

# es-distributed-server
A Distributed Server Framework Written in NodeJS 

The idea behind this concept is the following it reduces roundtrip times in large distributed Applications to reduce costs because less Servers and Services are needed for this structure.


# Some Examples
- NodeJS Listen for HTTP2 => POST Couchbase => Couchbase GET => RESPONSE
- NodeJS Listen for HTTP2 => POST KAFKA => KAFKA GET => RESPONSE
- NodeJS Listen for HTTP2 => POST Anything => Anything GET => RESPONSE

as you see in the examples there is some magic where is the processing? its a extra process thats the inovativ in this concept
The Concept it self is not new but there is One Big Paradigm Shift!!!! Normaly you would Process the request some where and then log it this goes directly the oposit way it logs it and then processes it.

I call this pattern GLPR Pattern Get Log Process Return where the Process is total decoupled. I Learnd this pattern from Database Engines and Tought about it often as i am a Database Hooligan i love what they do its magic :). This is used to archiv Fast Writes and Persistence.

This Repo will show you how to solve the big data challanges that do arrise via ECMAScript executed at present with NodeJS as it offers the most best runtime at present. Isolated and Scaleable via docker 

Oh By The way this is also the pattern that i use for my serverless http example because this pattern allows you to run serverless functions frictionless with advanced metrics and all the bells and withles

## The Secund Secret of this Implamentation
The Anything needs to get patched or should offer out of the box a hook for on('insert'|'modify'|CRUD) most best but optional locking would help on scale to squice out even more performance.

## The 3 secret is ?
Its caching the worker results for example by url as key and return that via a algorythm inside the worker. Sure you could add this directly to your http2 instances but that defeats the Log first algorythm so you gain speed and loose all the benefits of log first if you want to go that route you should do it rule based and only for content that is garantied to exist. Its often not worth doing that.





