# sovits-npu-mindtorch

## 原始readme
[**English**](./README_sovits.md) | [**中文简体**](./README_zh_CN.md)

### 开机

选择`mindtorch0.2_mindspore2.2.1_torchnpu2.1.0_cann7.0rc1`镜像
数据集勾选上`so-vits-svc-npu.zip`和你的数据集

### 解压程序、数据集&安装依赖&解决乱七八糟的问题

```shell
su
conda install -c conda-forge libsndfile -y
cp /dataset/* ./
unzip so-vits-svc-npu.zip
cp yourdataset.zip ./so-vits-svc-npu/dataset_raw
cd ./so-vits-svc-npu/dataset_raw
unzip yourdataset.zip
cd ..
pip install -r requirements.txt
```

### 重采样至44.1k
```shell
python resample.py
```