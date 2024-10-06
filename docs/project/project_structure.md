# 项目目录结构
## `docs`：源代码目录
### `docs/`下的文件夹
=== "`assets`：静态资源目录"
    用于存放图片、样式等静态资源
=== "`contest`：竞赛专区"
    - `introduction.md`:竞赛主页
    - `ICSD.md`:国际大学生工程力学竞赛分享
    - `zhoupeiyuan.md`:全国周培源大学生力学竞赛分享
=== "`coursesNav`：课程导航文件夹"
    - `index.md`:课程导航主页
    - `type.md`:课程类型导航
    - `courses_template.md`:**投稿提示**
    - `coursesdata.js`:用于生成课程目录的js文件，**课程目录的原数据也在js内**
    - `mechanics.md`:工程力学导航
    - `mechanics_strong.md`:工程力学（强基计划）导航
    - `mechanics_pro.md`:工程力学（拔尖班）导航
    - `aircraft_design.md`:飞行器设计与工程导航
    - `aircraft_design_excellent.md`:飞行器设计与工程（卓越人才培养班）导航
=== "`courses`：课程经验"
    !!! note
        每个文件夹下的md文件是单个课程的经验分享，文件名为课程名直译，如工程训练为`EngineeringTraining.md`，这类文件必须先在draft中写好留档，再移植到这里
    - `GeneralCompulsory`: 通识必修课程文件夹
    - `MajorCompulsory`: 专业必修课程课程文件夹
    - `MajorElective`: 专业选修课程文件夹
    - `MajorFoundation`: 通识选修课程文件夹
    - `.template.md`: 建设中课程的模板,之所以前面加点是为了防止mkdocs报错
    - `.courseLoad.js`: nodejs自动生成markdown树，并写入模板，之所以前面加点是为了防止mkdocs报错
### 其他`docs/`下的md文件
- `index.md`:主页
- `friend.md`: 友情链接
- `leap.md`: 飞跃手册
## `draft`: 草稿文件夹
初稿要先存放在这里，待完善后再移动到`docs`文件夹下，这类文件的标准写法请参看[课程分享标准写法](./courses_standard.md){:target="_blank"}
## `mkdocs.yml`
[mkdocs配置文件](./mkdocs_yml.md){:target="_blank"}