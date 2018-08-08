# 3SS2B ©

<img src="https://i.imgur.com/TDBAdNR.png" height="250"/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

An Android image fingerprint algorithm that uses 3SS to do downsize, greyscale, and fingerprint in one pass, and match images for similarity or distortion. Since we are using a modified dhash, it works for scale and aspect ratio changes already.  Similarity could also be defined by something like color or contrast changes.  I am experimenting to see how I can corelate two hashes as such using FMIQ, Haar transform, Radon fingerprinting, or Deep Autoencoders within Android.  I also may try to incorporate checks for rotation by obtaining additional fingerprints.

This is still in the experimental phase and under development, and hopefully the data will be turn out to be compatible on average.






## Best times for hashing, so far:

* JNI C++ nativeDHash: 

* Kotlin dHash: 



## License

* [Apache Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

## Building

This lib was built with Android Studio which uses the gradle build system.  

## Acknowledgements

This project uses the [Github API] ( https://www.github.com)

* http://www.hackerfactor.com/blog/?/archives/529-Kind-of-Like-That.html

* http://tech.jetsetter.com/2017/03/21/duplicate-image-detection/





