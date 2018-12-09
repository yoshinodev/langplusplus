# lang++
lang++ is a collection of code editing tools with support for non-English languages.

Most, if not all, of the world's widely-used programming languages are English-based, making it difficult for many non-English speakers to learn to code. Since computer knowledge and programming skills are becoming increasingly valuable in today's world, the lack of support for other languages puts non-English speakers at a disadvantage.

As of now, lang++ supports one language-programming language combination (Chinese-C++). We are currently working to increase number of languages, improve the use of links to external resources, and integrate machine learning to to provide better assistance to users.

## Instructions/Notes
To see the online editor demo in action, download ACE Editor files from ACE Github, index.html, and main.css (from "css" folder) files, then open index.html using browser. Or, go to [https://langpp.weebly.com](https://langpp.weebly.com).

Translation is in "translations" folder in the form of .csv file.

The data string in the demo is set to the string of Chinese-to-C++ translations (see [Chinese-C++ .txt file](https://github.com/fibanneacci/langplusplus/blob/master/translations/chinese_c_cpp.txt)), due to only having one language-programming language combination. In the future, we're aiming to make it dynamic (controlled using the dropdowns). In addition, we're working on improving our method of parsing translations from aforementioned .csv files; currently, we've been converting .csv files to .txt, then using the Python parse program in the "parse" folder to convert the data in the .txt file to one single string (with '\n' substituted for newlines).

## Goals for lang++

 * Add language-programming language combinations
 * Improve method for parsing translation data
 * Make demo dynamic
 * Incorporate machine learning
    * Improve translation accuracy
    * Consider context when suggesting autocompletions
    
## Contributing

Contributors to lang++ are involved in improving the code for the demo as well as integrating machine learning techniques to improve certain features including autocompletion. In addition, translations contributors are an integral part of lang++'s community. Please read [CONTRIBUTING.md](https://github.com/fibanneacci/langplusplus/blob/master/CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](https://github.com/fibanneacci/langplusplus/blob/master/CODE_OF_CONDUCT.md) to learn more about contributing to lang++.

## Built Using
* ACE Editor - online editor demo - [ACE Editor Github](https://github.com/ajaxorg/ace)

## Authors
* **Anne Li** - *Initial work* - [fibanneacci](https://github.com/fibanneacci)

## License
This project is licensed under the MIT License - see the [LICENSE](https://github.com/fibanneacci/langplusplus/blob/master/LICENSE) file for details
