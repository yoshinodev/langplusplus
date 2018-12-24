# lang++
A collection of code editing tools with support for non-English languages.

<img src="https://github.com/fibanneacci/langplusplus/blob/master/assets/demov.gif" width="650">

## ✔️ Purpose

Most widely-used programming languages are English-based, making the learning process difficult for many non-English speakers intending to use these languages in their studies and/or careers. lang++ addresses this issue using the translation functionality shown above.

## 🥅 Goals

 * Expand language-programming language translation database
   * As of now, lang++ supports only 1 lang-prog lang combination (Chinese-C++)
 * Improve method for parsing translation data / make data retrieval automated process
   * Currently, parsing involves using Python program to process .csv files (outputting data as single string)
   * String is then copy-pasted into html file as variable, parsed using D3
 * Incorporate machine learning
    * Improve translation accuracy
    * Consider context when suggesting autocompletions
    
See [issues](https://github.com/fibanneacci/langplusplus/issues) for detailed tasks and descriptions.

## 🗒️ Instructions

To see the online editor demo in action, follow these steps:

### ⬇️ Installation

1. Download ACE Editor files from ACE Github (See "Dependencies / Built Using" below)
2. Download D3 files from D3 Github (See "Dependencies / Built Using" below)
3. Download lang++ repository.

### 🏃 Usage

*Note: lang++ currently requires manual entry of translation data into the root html file. We are working to make this data retrieval an automated process.*
1. Open index.html using Notepad or any other text editor / code editor / IDE.
2. Find the following block of code (inside the "update_translations" function):

```javascript
        var data = "Chinese,cpp\n包括,#include\n包含,#include\n括,#include\n包,#include\n包罗,#include\n输入输出,iostream\n控制台输入输出,iostream\n标准输入输出,iostream\n文件输入输出,fstream\n运用,using\n用,using\n使用,using\n利用,using\n命名空间,namespace\n标准库,std\n整数,int\n数,int\n号码,int\n号,int\n主要,main\n主,main\n主干,main\n正,main\n接受输入,cin\n输入,cin\n接受控制台输入,cin\n控制台输入,cin\n接受标准输入输出,cin\n标准输入输出,cin\n从,for\n串,string\n弦,string\n线,string\n绳,string\n绳子,string\n字符,char\n字母,char\n字母字符,char\n浮点,float\n浮点数,float\n十进制,float\n小数点,float\n浮点数字,float\n双,double\n浮点,double\n浮点数,double\n十进制,double\n小数点,double\n浮点数字,double\n如果,if\n是否,if\n如,if\n假如,if\n要是,if\n若是,if\n倘若,if\n假若,if\n倘,if\n要,if\n假使,if\n否则,else\n除此以外,else\n不然,else\n要不然,else\n不然的话,else\n要不,else\n真正,true\n真,true\n真实,true\n属实,true\n确实,true\n实,true\n假,false\n虚假,false\n讹,false\n而,while\n正在,while\n直到,while\n一直到,while\n做,do\n办,do\n进行,do\n搞,do\n弄,do\n开关,switch\n交换机,switch\n断路器,switch\n交换器,switch\n输出,cout\n控制台输出,cout\n标准输出,cout\n文件流,fstream\n文件溪,fstream\n文件溪流,fstream\n文件河流,fstream\n输入文件流,ifstream\n输入文件溪,ifstream\n输入文件溪流,ifstream\n输入文件河流,ifstream\n输出文件流,ofstream\n输出文件溪,ofstream\n输出文件溪流,ofstream\n输出文件河流,ofstream\n打开,open\n开,open\n关闭,close\n关,close\n封闭,close\n关上,close\n返回值,return\n返回,return\n退回,return\n回,return\n退还,return\n类,class\n阶级,class\n类型,class\n种类,class\n用户定义的数据类型,class\n类,struct\n阶级,struct\n类型,struct\n种类,struct\n用户定义的数据类型,struct\n私人的,private\n私人,private\n私营,private\n私有,private\n私,private\n私立,private\n公共,public\n公众,public\n公开,public\n公,public\n保护,protected\n防护,protected\n向量,vector\n动态数组,vector\n别号,typedef\n新名字,typedef\n其他名字,typedef\n用户指定的名称,typedef\n对,pair\n双,pair\n一对,pair\n组,set\n集,set\n集合,set\n一套,set\n套,set\n多集,multiset\n堆,stack\n先排在后面,stack\n先进后出,stack\n队列,queue\n先进先出,queue\n优先队列,priority_queue\n地图,map\n图,map\n字典,map\n词典,map\n辞典,map\n辞书,map\n无序的地图,unordered_map\n无序的图,unordered_map\n无序的字典,unordered_map\n无序的词典,unordered_map\n无序的辞典,unordered_map\n无序的辞书,unordered_map\n算法,algorithm\n分类,sort\n类,sort\n捃,sort\n整理,sort\n找,find\n寻找,find\n找,find\n搜寻,find\n搜索,find\n发觉,find\n薮,find\n极少,min\n最低,min\n最低限度,min\n最小值,min\n最大值,max\n最大,max\n极大,max\n数学,math.h\n数学头文件,math.h\n数学,cmath\n数学头文件,cmath\n反余弦,acos\n反正弦,asin\n反正切,atan\n反正切,atan2\n天花板,ceil\n顶棚,ceil\n潼,ceil\n最小数量大于,ceil\n余弦,cos\n双曲余弦,cosh\n加,+\n减,-\n乘,*\n除,/\n除,div\n除,ldiv\n加法,+\n减法,-\n乘法,*\n除法,/\n除法,div\n除法,ldiv\n指数,exp\n绝对值,abs\n绝对值,fabs\n绝对值,labs\n地板,floor\n地面,floor\n地,floor\n最大数量少于,floor\n模,%\n模,fmod\n大数,long\n大的数,long\n长,long\n长数,long\n大数,long long\n大的数,long long\n长长,long long\n长长数,long long\n对数,log\n对数,log10\n基数10对数,log10\n分解,frexp\n重建,ldexp\n分解,modf\n分解数,frexp\n重建数,ldexp\n分解数,modf\n分解数字,frexp\n重建数字,ldexp\n分解数字,modf\n指数,pow\n正弦,sin\n双曲正弦,sinh\n平方根,sqrt\n随机,rand\n任意,rand\n切线,tan\n双曲正切,tanh\n底线,endl\n新队,endl\n新线,endl\n回车,endl"
        var parsed = d3.csvParse(data);
        var dict = {};
        for (var i = 0; i < parsed.length; i++) {
            dict[parsed[i].Chinese] = parsed[i].cpp;
        }
        //add custom completer w/ translations
        var wordList = [];
        for (var i = 0; i < parsed.length; i++) {
            wordList.push(parsed[i].Chinese);
        }
```

3. Replace string in "data" variable with string for your preferred translations. Do so by following these steps:
    1. Open program "parse.py" (in "parse" subdirectory).
    2. Replace file name in line 1 with name of file containing your preferred translations (should be in the format "Lang_proglang.txt").
    3. Run program and copy output into "data" variable (if you do not have Python compiler installed on your computer, use online compiler such as [OnlineGDB](https://www.onlinegdb.com/online_python_compiler), copy and paste code into "main.py", and create .txt file containing translations in .csv format using the "New File" button)
4. Replace all instances of "Chinese" with your preferred language, and "cpp" with your preferred programming language.

*"index.html" in Google Chrome:*

<img src="https://github.com/fibanneacci/langplusplus/blob/master/assets/demo.png" width="650">

You can find translations in the "translations" folder, in the form of .csv files (easy to view and edit) and .txt files (single string outputted by parsing program).
    
## 👥 Contributing

lang++ provides various opportunities for contributing, including:

 * Expanding the database of translations
 * Improving the demo code
 * Integrating machine learning

We greatly appreciate contributions; yours will not go unnoticed. Please visit [contributors](https://github.com/fibanneacci/langplusplus/contributors) to view a list of contributors this project. Read [CONTRIBUTING.md](https://github.com/fibanneacci/langplusplus/blob/master/.github/CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](https://github.com/fibanneacci/langplusplus/blob/master/CODE_OF_CONDUCT.md) to learn more about contributing to lang++.

## 🛠️ Dependencies / Built Using
* ACE Editor - online editor demo - [ACE Editor Github Repo](https://github.com/ajaxorg/ace), [Official Website](https://ace.c9.io)
* D3 - parsing .csv data - [D3 Github Repo](https://github.com/d3/d3), [Official Website](https://d3js.org)

## ✍️ Author
* **Anne Li** - *Initial work* - [fibanneacci](https://github.com/fibanneacci)

View [contributors](https://github.com/fibanneacci/langplusplus/contributors) to this project.

## ⚖️ License
This project is licensed under the MIT License - see the [LICENSE](https://github.com/fibanneacci/langplusplus/blob/master/LICENSE) file for details.
