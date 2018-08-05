# 3SS2B ©

<img src="https://i.imgur.com/TDBAdNR.png" height="250"/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

An Android dhash algorithm that uses 3SS to do NN, greyscale, and fingerprint in one pass, and match images for similarity using a modified Hamming distance algorithm. Since we are using a modified dhash, it works for scale and aspect ratio changes already.  Similarity would be defined by something like color or contrast changes.  I am experimenting to see how I can colrelate two hashes as such.  I also may try to incorporate checks for rotation by obtaining additional fingerprints.

I use bit filtering techniques such as bit count in a garbage free map structure and/or a bloom filter for exclusion. In any   dataset that can get a hash to match duplicates, this changes an O(n) search to one on O((epsilon * 2)+1) buckets in the map, or across that many rows in the db.  Since epsilon is usually quite small (~2), it is potentially constant amount of work for each image. This is still in the experimental phase and under development, and hopefully the data will be turn out to be compatible on average.






## Best times for hashing, so far:

* JNI C++ nativeDHash: 

* Kotlin dHash: 



## License

* [Apache Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

## Building

This lib was built with Android Studio which uses the gradle build system.  

## Acknowledgements

This project uses the [Github API] ( https://www.github.com)
http://www.hackerfactor.com/blog/?/archives/529-Kind-of-Like-That.html
http://tech.jetsetter.com/2017/03/21/duplicate-image-detection/





