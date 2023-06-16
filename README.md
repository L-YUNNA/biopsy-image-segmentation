# biopsy-image-segmentation

조직 검사 이미지를 segmentation 하기 위해 다음 두 가지 방법을 사용하였다. <br><br/>
1. openCV - cv2.kmeans, cv2.inRange, cv2.GaussianBlur, cv2.threshold 등의 기능 활용
2. SAM (segment anything) - foundation model 사용 <br><br/>
<br><br/>
## Segment anything
분할하고자 하는 영역(또는 제외할 영역)에 대한 포인트(prompts)를 줘서 segmentation.


추후 분할된 mask를 사용하여 line of interest and patches를 얻고자 함 (cv2.getStructuringElement, cv2.dilate)
<br><br/>
<br><br/>
## Reference
**Segment Anything** 


paper : https://arxiv.org/abs/2304.02643
github : https://github.com/facebookresearch/segment-anything/tree/main#citing-segment-anything
demo : https://segment-anything.com/ 
