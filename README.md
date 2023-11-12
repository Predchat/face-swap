# Face Swapping With Deep Fakes Methods

<div align="center">

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/sabahesaraY)

[![Twitter](https://img.shields.io/twitter/follow/sabahesaraki?style=social)](https://twitter.com/saba_hesaraki)

</div>

## Face Swap For Images Results
<div>
<img src="https://github.com/saba99/Face_Swap/assets/33378412/80d1507e-be8e-4f5d-be6d-acb7caca8447">
<img src="https://github.com/saba99/Face_Swap/assets/33378412/b69da8d8-48e4-45f9-ba99-b4c33b04de12">
<img src="https://github.com/saba99/Face_Swap/assets/33378412/ac846aae-4686-4461-9a56-4df0ddbf2ba5">
<img src="https://github.com/saba99/Face_Swap/assets/33378412/f9309cc9-f746-48b7-bbac-8d85658d1081">
 
</div>


## Installation
  
1. Clone this repository
  ```bash
  git clone https://github.com/saba99/Face_Swap.git
  cd Face_Swap

  ```
2. Install dependent packages
  ```bash
  pip install -r requirements.txt
  ```
  
3. Download weights
  ```bash
  sh download_models.sh
  ```
## Face Swap On Video

  1.download Face Video From this link [[Face Videos](https://www.pexels.com/search/videos/face/)] 
 

  2. Face Swap On Video
  
  Swap to one specific person in the video. You must set face from the target video (for example, crop from any frame).
  ```bash
  python inference.py --source_paths {PATH_TO_IMAGE} --target_faces_paths {PATH_TO_IMAGE} --target_video {PATH_TO_VIDEO}
  ```
  Swap to many person in the video. You must set multiple faces for source and the corresponding multiple faces from the target video.
  ```bash
  python inference.py --source_paths {PATH_TO_IMAGE PATH_TO_IMAGE ...} --target_faces_paths {PATH_TO_IMAGE PATH_TO_IMAGE ...} --target_video {PATH_TO_VIDEO}
  ```
 ## Face Swap On Image
  
  You may set the target face, and then source will be swapped on this person, or you may skip this parameter, and then source will be swapped on any person in the image.
  ```bash
  python inference.py --target_path {PATH_TO_IMAGE} --image_to_image True
  ```
