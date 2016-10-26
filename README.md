笔顺数码输入法码表 stroke-seq_MB 第一版 v1
    
    版权：GPL v3+
    遵照《GB13000.1字符集汉字字序（笔画序）规范》共20902个汉字
    遵照《GB13000.1字符集汉字笔顺规范》
    遵照2013年6月印发的《通用规范汉字表》8100个简体繁体异体字对照表
    基于专利权已终止的（CN03159505.7）“一种数字笔画汉字输入方法”
    参考《数字五笔中文输入系统输入教程及编码查询手册》原发明人：马晓光 <232937@QQ.com>
    开源码表手工录入、修改并简化规则、边旁部首（部件）编码全部重排：一善鱼 YQ-YSY <YQ-YSY@163.com>
    欢迎各位朋友利用此码表，或开发独立的笔顺输入法，或嵌入已开发的输入法。
    为了方便大家编辑并导出码表，在此使用原始的LibreOffice电子表格ods文件，里面有详细的分类编号及排序。
    
* * *
    
<big>按键说明</big>
    
    笔顺数码输入法使用键盘数字小键盘为主要输入工具，单手即可完成简体繁体文字、词组以及标点符号的输入。
    输入速度快，重码极少，适合编写长篇文章、会议速记等工作，符合华人书写习惯，避免“提笔忘字”的电脑病。
    
    小键盘的0~9按键默认是录入汉字，若先输入“*（星号）”紧接着输入0~9则为录入数字；
    按键“/（斜杠号）”单独输入时为逗号，
    按键“*（星号）”单独输入时为切换到数字输入模式，若跟随在编码后输入则作为未知编码的模糊查询通配符；
    按键“-（减号）”为撤销上一步按键（类似BackSpace向左退格键）；
    按键“+（加号）”单独输入时为+号，若跟随在编码后输入则切换到候选字选词模式，继续输入0~9选择列出的字词；
    按键“Enter（回车）”用于确认选中排在第一个的候选字词就是需要的字词；
    按键“.（点号）”单独输入时为逗号，若跟随在编码后输入则作为词组的汉字间隔符；
    按键“00”为列出标点符号候选；按键“09”为列出特殊数字序号候选。
    
    大键盘上的其它按键，与其它输入法功能相同。例如：
    -号或者 PageUp 候选字词向上翻页；=号或者PageDown 候选字词向下翻页；
    Shift 4 为￥人民币符号，Shift 6 为……省略号，shift < 为书名号《，以及 Ctrl . 为全角半角切换等。
    为了方便没有数字小键盘的笔记本用户，建议输入法开发者提供自定义按键替换0~9的功能，以及繁体简体互换功能。
    
<big>显示说明</big>
    
    输入法悬浮栏的显示方式，建议输入法开发者参考原“数字五笔输入法”分两行提示框的显示方式，方便用户学习记忆。
    用户输入编码时：
    已输入的数字、其所代表的笔画、以及所代表的字首部件显示在悬浮栏第一行（提示框），不需要死记硬背，即可看见。
    候选字列表显示在悬浮栏第二行（候选框）。编码输入完毕，用户选择了所需要的字之后：
    悬浮栏第一行显示刚才这个字、词的“精简码”、“六全码”，方便用户学习记忆。
    第二行显示最近经常输入的句子或短语以供重复输入，或者联想词组以供快速输入。
    输入法悬浮栏应当还提供有其它帮助按钮，方便用户进行查看部件编码表，或者进行相关设置。
    
* * *
    
<big>一、笔顺码</big>
    
    以1、2、3、4、5五个数字分别代表“一丨丿丶乛”五个笔画，按汉字笔顺进行输入。其中：
    “提”归为“一”：如“氵、扌”中的最后一笔；
    “亅”归为“丨”：如“小”字的第一笔；
    “点、捺”归为“丶”：如“文、入、表”的最后一笔；
    各种折笔（乛、乚、、⺄、弯钩、竖提等）都归为“乛”：如“为、孔、民”中的笔画。
    
    例如：
    “开”字，按笔顺“一、一、丿、丨”，编码为1132；
    “我”字为31；“向”字为325；“力”为53；
    注意“万”为153，“方”为4153，“忄”为442。
    一般说来，常用字只需输1~4、5码。
    
    标点符号输入：
    常用标点符号可以输入“00”,常用的数字序号可以输入“09”。
    
* * *
    
<big>二、六全码、精简码</big>
    
    使用二个数字的组合来代表汉字中的边旁部首或部件，注意每个部件必须严格按笔画顺序排列，不得跨越笔顺拆解部件。
    每个汉字最多取六个编码，当汉字编码超过六个时，第六码取该汉字最后一笔编码，
    若该字最后一部分为常用部件，则取该常用部件的最后一笔编码。例：
    
    尘：23419（"尘"的前三笔是竖丨、撇丿、点丶、编码234，后三笔为常用部件"土"，编码19。）
    镜：916085（"镜"的钅为91,立为60，日为80，儿已经超六码，最后一笔为"折乛"，因此第六码取5，不取0。）
    梦：121234（"梦"的两个木为1212,夕为354，但已经超六码，因此保留最后一笔"点丶"4，不取5。）
    再：125211（"再"最后三笔虽然像是一个“土”字，但按笔顺则应该是先一竖再二横，因此不能取“土”作为部件）
    回：25801 （"回"字不能拆解为二个“口”，因为按笔顺外面大“口”的最后一笔要等小“口”写完后才能封口）
    
    六全码目前一共录入了《GB13000.1字符集汉字字序（笔画序）规范》20903+8个汉字，包括繁体字、异体字、以及日韩所用的汉字。
    精简码则是六全码的简化格式，包括了《通用规范汉字表》一级二级汉字和部分三级汉字，1~6键即可快速打出最常用的个汉字。例：
    
    我：简码为31，  全码为312154；
    自：简码为382， 全码为382；
    无：简码为1135，全码为1135；
    心：简码为65，  全码为65；
    是：简码为8，   全码为811214；
    
    大多数常用的汉字，均不需取完所有六个编码便可出现在候选汉字的首位，然后按回车键直接完成输入，
    处在候选列表的汉字，只需在小数字键盘里，按下+号，再按数字键，即可选中候选列表里的汉字。
    由于有极少部分精简码与六全码完全相同，请输入法开发者把精简码所代表的常用汉字排在候选列表靠前的位置。
    
<big>三、部件编码表</big>
    
    利用"1、2、3、4、5"代表部件笔画"横一、竖丨、撇丿、点丶、折乛"，
    利用"7、8、9、6、0"代表部件笔画"横一、竖丨、撇丿、点丶、折乛"，
    在键盘上输入方位类似的二个0~9按键，就能得到各种常见的的边旁部首和部件。在数字小键盘上的排列如下：
        
    7横一  8竖丨  9撇丿
    4点丶  5折乛  6点丶
    1横一  2竖丨  3撇丿
    0折乛        .
    
    不需要死记硬背，因为在输入第一个数字后，提示框中会出现这个数字开头的的偏旁部首（部件）列表，一看便知，打字多了自然就记住了。
    如果需要输入的汉字刚好就是这个部件，那么只需要输入这个部件编码即可；若一个部件代表多个汉字，则再加几个0即可在候选列表中找到。
    笔画数较少多、常用、结构简单的边旁部首和部件（共50个）：
    
    10 扌 11 二王  12 十丅丁木朩  13 厂丆歹豕（有字头）   14 石   15 七丂匚匸   16雨    17 艹⺿  18 廿  19 土士走
    20 山    21 丄止歺   22 刂业   23 非   24 卜⺌  25 冂巾（有字底）    26 虫   27 且（直字底）  28 贝貝  29 ⻊足
    30 饣飠食  31 牜牛   32 亻   33 彳   34 八人入乂  35 九几儿匕勹角（然字边）  36 月   37 ⺮   38 犭   39 爫豸
    40 讠    41 冫亠方   42 门   43 丷兰    44 氵   45 冖    46 宀    47 广   48 疒   49 忄
    50 马馬   51 刁巳   52 了阝卩丩凵   53 刀力乃   54 又厶廴（予字头） 55 纟糹  56 幺   57 弓   58 子孑   59 女
    
    笔画数较多、不太常用、结构复杂的边旁部首和部件（共46个）：
    
    70 其   71     72 丅耳    73丰耒（邦字边）   74 西覀    75 酉   76 冓字头  77 车車   78 镸髟   79（无）
    80 口     81 日曰    82 目   83 田由甲申   84 罒四皿    85 骨     86 門鬥    87 虍    88（无）   89（无）
    90 夂攵（祭字头）91 钅釒金  92 禾   93 ⺁舟彡  94 矢  95 鬼   96 舌   97 片身臼（段舆盥字边） 98 鱼魚  99 鸟鳥
    60 立（旁字头中）61 訁言   62 礻   63 衤  64 兴字头   65 心必   66 文六   67 手毛气   68 米（敝字旁） 69 火灬
    00（标点符号）01 彐（录肀字头那字边）02 爿 03 艮（即字旁）04 习羽  05 乜彑毌母  06 巜巛  07 尸 08 癶 09（数字序号）
    
    部件编码的规则是以汉字笔顺为准，优先选用汉字起头的边旁部首，原本就是二个笔画的边旁部首也尽量保持在与笔顺编码相同的原位。
    少数部件按视觉、听觉形成的思维习惯、以方便记忆为目的，进行编码排列。
    由于某些部件没有相对应的单个汉字，在此以“某字边、某字头”来说明，请输入
    法开发者在制作提示框时，改为用图片显示正确的部件形式。
    
    只需一个编码，即 0~9 所代表的最常用汉字分别是：
    1 一，2 国，3 的，4 为，5 能，6 这，7 要，8 是，9 和，0 那。
    如果记不全某个汉字的六全码或者笔顺码，可以在输入第一个编码之后，使用“*（星号）”作为该字未知编码的模糊查询通配符。
    例如：记不全“镜”这个字的六全码,只记得第一个和其中两个编码：可以输入9*08*，或者9*5就可以在候选字列表中找到“镜”字。
    注意，如果按键“*（星号）”作为第一个输入按键，则切换到数字输入模式。
    例如：想输入数字123，就只需在数字小键盘输入*123回车即可。
    
    六全码或精简码也可以打出繁体字，某些繁体字与简体字编码相同的，目前是默认排在简体字后面。
    习惯使用繁体字输入的用户，可以在单字码表的基础上重新排列优先字序，让某些繁体字与简体字编码相同的，默认排在简体字前面。
    也希望输入法开发者能做出一个“繁体/简体“转换按钮，或者一个”汉字信息“按钮，用来显示这个汉字完整笔顺、拼音、内码等信息。
    
* * *
    
<big>四、词组输入规则</big>
    
    词组中的每个字之间用“.”（点号）隔开即可，用户可以输入自己记得的不定长的编码。词组码表只有六全码和笔顺码即可。
    唯一要注意的是词组的每个字的编码必须统一，即：第一个字用六全码或精简码，后面的字就不能混用笔顺码，反之亦然。例如：
    中国：85.257（六全码）或 25.251 （笔顺码）
    汉武帝：64.22.67（六全码）或 441.22.414（笔顺码）
    
    虽然词组中每个字可以输入任意长度的编码，但建议每字输入2－3个编码，这样更有利于精确定位词组，减少选词的麻烦。
    多字超长词组的输入十分简单，只输入词组两头的汉字编码，中间要省略的多个字直接用一个“.”（点号）隔开即可。例：
    中华人民共和国：85.32..25（这时，候选列表会显示出“中华人民共和国”和“中华民国”两个词组）
    百闻不如一见：13..1.25（注意不能输入 13..13..25 即：中间不能省几字、又加一字、又省几字。只能用两头、省中间。）
    
    如果记不全词组中某个汉字的编码，可以在输入第一个编码之后，使用“*（星号）”作为该字未知编码的模糊查询通配符。
    例如：记不全“汉武帝”这三个字的六全码,只记得第一个和其中两个编码：
    可以输入6*.*4.6*，或者6*.*.*5就可以在候选字列表中找到“汉武帝”这个词组,所记得的编码越多，查询越准确。
    
    建议输入法开发者能参考“搜狗词库”的管理方式，利用单字码表生成多种分类词汇码表，并提供在线更新，以增强本输入法的生命力。
    也希望输入法开发者能开发出“自造词组”的功能，以及上次经常输入的句子短语的记忆功能，这能为用户的输入体验带来极大的方便。
    习惯使用繁体字的用户也许需要生成专门的繁体字词组码表，或者开发一个“繁体/简体“转换按钮。
    
* * *
    
<big>    六、易错易混汉字</big>
    
    以下汉字是容易输入错误或混淆的：
    1、"末、未、果"等后四笔形成的"木"形结构，其结构清晰，易于辨认，且笔画顺序与"木"相同，故取"木"的编码12；
    2、"都、教、考、孝"等前三笔形成的"土"形结构，其结构清晰，易于辨认，且笔画顺序与"土"相同，故取"土"的编码19；
    3、"截、戴、载、裁"等前三笔虽也形成"土"形结构，但变形严重，不易辨认，故需按其笔顺取码121；
    4、"国、因"等含"囗"的汉字，因按笔顺这些字最后才封口，故不取"口"；正确取法，第一、二笔取"丨、乛"，取码25；
    5、"甘、某"等的开头几笔形成的结构即非"艹"字头，也非"廿"头，需按其笔顺取码122；
    6、"里、垂、重"等最后三笔形成的"土"形结构，因其笔顺是先一竖再横，与"土"字旁不同，故需按其笔顺取笔画编码（”里“取”甲“部件）；
    7、"衰、蓑"等字中间的"口"形结构，按笔顺应先写"口"中间的一横，打乱了"口"字的笔顺，故不按"口"字部件取码，需取其笔画编码2511；
    8、"缶、击、出"等字最后三笔形成"山"形结构，笔顺也与"山"相同，但不易于辨认，故不取"山"字旁，需取笔画编码252；
    9、"制，刺，敝"等的左边均有类似"巾"的结构，笔顺也与"巾"相同，但不易于辨认，故不取"巾"字旁，需取笔画编码252；
    10、“冒、帽”上面不是“日”字，而是丨乛一一，这两横不连接到旁边，即2511。
    11、”有、育、膏“的下面不是”月“，而是先一竖丨乛一一，即2511（简码25）。
    
    以下汉字和部件的笔顺容易出错：
    七：一乛 15              九：丿乛 35
    匕：丿乛 35              乃：乛丿53
    刀：乛丿 53              力：乛丿 53
    万：一乛丿 153            小：丨丿丶234
    及：丿乛丶 354            忄：丶丶丨442
    义：丶丿丶 434            车：一乛一丨1512
    巨：一乛一乛 1515         比：一乛丿乛 1535
    瓦：一乛乛丶 1554         牛：丿一一丨 3112
    牜：丿一丨一 3121         长：丿一乛丶 3154
    方：丶一乛丿 4153         火：丶丿人 4334
    为：丶丿乛丶 4354         丑：乛丨一一 5211
    爿：乛丨一丿 5213         办：乛丿丶丶 5344
    毋：乛乛丿一 5531         世：廿乛 12215
    可：一口丨 12512          龙：一丿乛丿丶 13534
    北：丨一一丿乛 21135       凸：丨一丨乛一 21251
    由：丨乛一丨一 25121       冉：丨乛丨一一 25211
    凹：丨乛丨乛一 25251       必：丶乛丶丿丶 45434
    讯：讠乛一丨 45512         出：乛丨丨乛丨 52252
    皮：乛丿丨又 53254         母：乛乛丶一丶 55414
    考：土丿一乛 121315        兆：丿丶一乛丿丶 341534
    那：乛一一丿阝 511352       里：日丨一一 2511211
    卵：丿乛丶丿卩丶 3543524    非：丨一一一 丨一一一 21112111
    官：宀丨乛一乛一 44525151   肃：乛一一丨丿丨八 51123234
    贯：乛乛丨一贝 55212534     重：丿一日丨一一 312511211
    脊：丶一丿丶人丨乛一一 4134342511
    衰：丶 一丨乛一一丿乛丿丶 4125113534
    曹：一丨乛一丨丨一日 12512212511
    爽：一丿丶丿丶丿丶丿丶人 13434343434
    兜：丿日丿乛乛一丿乛 32511355135
    敝：丶丿丨乛丨丿丶攵 43252343134
    舆：丿丨一一车乛一一一丿丶 32111512511134
    噩：一丨口口一口口一 1225125112512511
    再：一丨乛丨一一125211
    