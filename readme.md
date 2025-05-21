#### 说明
- Release_OcrModule 下是编译出的x32 dll和引入库
- Release_TestOcrDll下 是一份x32 ObssOcrModule.dll测试工具，其中含有需要的各dll和模型等文件
- Release_TestOcrDll\jsondemo输出供参考.json 是dll调用输出，供参考
- TestOcrModule\obss_ocr_api.h 是ObssOcrModule.dll的 函数声明，dll 隐式链接可用，其中有调用约定和各参数的说明

####  Release_TestOcrDll 下的测试工具使用示例

```
 cd Release_TestOcrDll
 .\TestOcrModule.exe models\ch_ppocr_mobile_v2.0_det_infer.nb models\ch_ppocr_mobile_v2.0_rec_infer.nb models\ch_ppocr_mobile_v2.0_cls_infer.nb images\tiket.jpg output\tiket.jpg models\assets\ppocr_keys_v1.txt models\assets\config.txt
```