# Clara - Pancreas Classification

## Docker
docker -t [name]

--rm => "exit" to logout

docker ps

GPU編號

before enter docker, check the use of GPU

In docker-nvidia, 
   1. Nvidia_visible_device={index}
   2. -v =>like the gcc -l(or -L), {outer path}:{inner substituted path}

    
~~[TODO] (tinghui) 新增名稱~~
[TODO] (all) try CLARA_VERSION 改成 3.0
[TODO] -v 項目確認 (放code?放data?)

---

## Preprocessing
### Data
- [ ] todo
Data description:
1. link : work/pancreas/clara/dataset(quiker than open from data2)
2. process => temporary storage
    1. raw(from data2, nifti, ) -> resample(constructed by resample.sh) -> crop
    2. -l =>label without resample(in resample.sh)
    3. if call afezeria/... =>clara sampel function
3. dataconvert.py => the specific clara function is 
3. classification=> final data form
    1. How clara fit the data into the model 
         (1). root path (2) *json

[TODO] (tinghui) finish datacustom.py
[TODO] eliminate the warning of crop.py
[TODO] (tinghui) try resample [a, a, a] to [a, b, c]
~~[TODO] (tinghui) crop.py 改成 input image path and label path~~
[TODO] (chingwen) crop.py 加入 erosion/dilation function, maybe add test
[TODO] crop.py 加入 crop 多少
[TODO] (tinghui) generate json

afezeria => sample code

