# 3SS2B ©

<img src="https://i.imgur.com/TDBAdNR.png" height="250"/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

An Android dhash algorithm that uses 3SS to do NN, greyscale, and fingerprint in one pass, and match images for similarity using a modified Hamming distance algorithm. Usually, the epsilon would be found in practice by calculating XOR of two fingerprints and setting a bound on how many set bits may vary. Instead, I use bit filtering techniques such as a bit count using MIT's fast MEMHACK bitwise algorithm in a garbage free map structure and/or a bloom filter for exclusion. In certain datasets this may suffice but additional techniques such as distribution masking can be added. This changes an O(n) search for each image into an O((epsilon * 2)+1) number of constant time buckets in the map, which may turn out to be sparsely populated. Since epsilon is usually quite small (~2), it is potentially constant amount of work for each image. This is still in the experimental phase and under development, and hopefully the data will be turn out to be compatible on average.






## Best times for hashing, so far:

* JNI C++ nativeDHash: 

* Kotlin dHash: 



## License

* [Apache Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

## Building

This lib was built with Android Studio which uses the gradle build system.  

## Acknowledgements

This project uses the [Github API] ( https://www.github.com)





