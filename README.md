# Description
This repository is a snapshot of image_common rolling branch commit [fd51363](https://github.com/wvu-urc/image_common/commit/fd51363e2b8f8cd99e9a77970c1d49eb86c1480f) modified to work in a humble environment. It was used because it has a fix that allows image_transport to properly decompress theora streams

# Known Limitations
Must be held in seperate workspace away from other code or all other launches fail. This is most likely due to it having the same name as the ros2 image_common package (because it is a paired down version of that)
This repository does not have all of the image_common features, and it's only intended use is to decompress theora streams
Theora streams have their own limitations that are handled using additional packages in the main workspace
