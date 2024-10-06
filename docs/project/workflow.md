# 工作流
## 无Git课程书写
1. 创建空Mkdocs项目，具体做法：[本站Mkdocs教程](../tutorial/mkdocs.md){target="_blank"}
2. 把项目mkdocs.yml的内容复制到对应mkdocs.yml文件中
3. 在docs目录下任意创建.md文件寻找相应资料开始整理书写（过程中通过网页查看写作效果）[书写规范](courses_standard.md){target="_blank"}
4. 整理完成后，把.md文件发送给可以进行Git的同事，由ta帮助上传整理
5. 进行相应的登记

## 有Git课程书写
1. 直接从ZJU Git获取项目，要完成环境配置
2. 开始写作前在群里说明要写作的课程，避免冲突！
3. 在draft目录下创建正确文件名的markdown，开始整理书写（过程中通过网页查看写作效果）[书写规范](courses_standard.md){target="_blank"}（如果有人把md传给你，也请你合并在draft下）
4. draft完成后整理至对应的courses下的文件，并在draft中用注释写明“已加入版面”！如果是产生修改，在完成修改前要把注释去掉！
5. draft书写完毕即可排版至courses下
6. 不论是仅仅完成draft还未排版至courses下，还是已经排版至courses下，都要可以进行pull、commit、push操作，commmit信息写明“日期，完成内容，操作人（可以用简称）”
7. 解决冲突的时候一定要汇报！
8. 进行相应的登记，有能力的同学可以尝试进行课程信息更新

## 课程信息更新（需要Git）
1. 打开courseNav/coursesData.js
2. 找到coursesAll变量中的课程名对应的内容，更新课程信息（大部分情况都是更新加*的内容）：
```json
{
    "name": "课程名",
    "credit": 3,//学分，不用改
    "difficulty": 0,//*难度，从1开始数分别是水/略学/考前突击/长期努力/捞捞/死/抽象，可以根据几篇投稿酌情判定
    "term": "一(秋冬)",//建议学年学期
    "status": "建设中",//*建设状态，有n篇完整就写n篇完整，还可以加上较新较旧等形容
    "id": 0,//唯一识别ID，不用改
    "type": "通识必修课程",//类型，不用改
    "path": "GeneralCompulsory/LinearAlgebraIH"// 路径，不用改
}
```
3. 保存并提交，如果遇到冲突要妥善处理！最好在群里说明！

## 建设中的课程模板修改（需要node.js环境）
1. 打开`courses/.template.md`修改需要修改的部分
2. **检查课程信息更新是否已经完成，并且在群中询问**
3. 打开`courses/.courseLoad.js`把coursesAll变量中的内容替换成`coursesNav/coursesData.js`中的coursesAll变量，**程序运行后“建设中”的课程将会被写入.template.md文件的内容**
4. cd 至`courses`目录下，运行`node .courseLoad.js`，看到文件树建立成功的提示说明已经完成。