# 3SS2B ©

<img src="https://i.imgur.com/TDBAdNR.png" height="250"/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

An Android dhash algorithm that uses 3SS to do NN, greyscale, and fingerprint in one pass, and match images for similarity using
a modified Hamming distance algorithm.
Traditionally the epsilon would be found in practice by calculating XOR of two fingerprints and setting a bound on how many set bits 
may vary.  Instead, I keep track of each fingerprint's set bit count using MIT's fast MEMHACK bitwise algorithm in a garbage free
map structure.  This changes an O(n) db search for each image into an O((epsilon * 2)+1) number of constant time checks in the map.
Since epsilon is usually quite small (~2), it is constant amount of work for each image.
This is still in the experimental phase and under development.





## Best times for hashing, so far:

* JNI C++ nativeDHash: 

* Kotlin dHash: 



## License

* [Apache Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

## Building

This lib was built with Android Studio which uses the gradle build system.  

## Acknowledgements

This project uses the [Github API] ( https://www.github.com)





