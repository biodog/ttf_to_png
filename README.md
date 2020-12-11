

## requirement

- fonttools
- pillow


## 用法

```bash
python3 ttf_2_png.py -f test.font
```

## 参数

-f 字体文件(必需)

-o 输入图片保存目录

-s 图片大小

## 有字体反爬的网站

字体加密已经成为一种比较常见的反爬方式,下面的网站已经采用了字体加密的方式

1. 猫眼电影 https://maoyan.com/ 票房等数据
2. 黄页88 http://b2b.huangye88.com/ 企业联系电话
3. 中国土地市场网 https://www.landchina.com/
4. 大众点评
5. 起点中文网,https://book.qidian.com/info/1013562540 作品字数
6. 汽车之家
7. 实习僧 https://www.shixiseng.com/intern/inn_zq8poavkguii 

## 解决字体反爬的常用思路:

1. 获取字体文件,通常为ttf文件,woff文件或base64编码的形式
2. 查看字体文件内容,获取映射关系
3. 替换源文件中的内容,实现解密
