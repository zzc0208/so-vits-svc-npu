# sovits-npu-mindtorch

## 原始readme
[**English**](./README_sovits.md) | [**中文简体**](./README_zh_CN.md)

###解压程序、数据集&安装依赖

```shell
su
cp /dataset/* ./
unzip so-vits-svc-npu.zip
cp yourdataset.zip ./so-vits-svc-npu/dataset_raw
cd ./so-vits-svc-npu/dataset_raw
unzip yourdataset.zip
cd ..
pip install -r requirements.txt
```