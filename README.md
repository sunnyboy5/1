# Python笔记（B站——主播林粒粒呀）https://lqmboy.lanzouu.com/in4mK2r8dykf

```python
print("Dad!")
print("妈！！"
```

```python
print("你好" + " 这是一句代码" + " 哈哈")

print('Let\'s go')
print("\n")
print("我是第一行\n我是第二行")

print("""君不见，黄河之水天上来，奔流到海不复回。
君不见，高堂明镜悲白发，朝如青丝暮成雪。
人生得意须尽欢，莫使金樽空对月。
天生我材必有用，千金散尽还复来。
烹羊宰牛且为乐，会须一饮三百杯。
岑夫子，丹丘生，将进酒，君莫停。
与君歌一曲，请君为我倾耳听。
钟鼓馔玉不足贵，但愿长醉不复醒。
古来圣贤皆寂寞，惟有饮者留其名。
陈王昔时宴平乐，斗酒十千恣欢谑。
主人何为言少钱，径须沽取对君酌。
五花马，千金裘，呼儿将出换美酒，
与尔同销万古愁。""")
```

```python
greet = "您好，吃了么，"
greet_chinese = greet
greet_english = "Yo what's up, "
greet = greet_english
print(greet + "张三")
print(greet + "李四")
print(greet + "王五")
print(greet_chinese + "张三")
```

```python
import math
print(math.floor(3.5))
```

```python
port math

a = 1
b = 9
c = 20
delta = b ** 2 - 4 * a * c
print((-b + math.sqrt(delta)) / (2 * a))
print((-b - math.sqrt(delta)) / (2 * a))
```

```python
# 对字符串求长度
s = "Hello world!"
print(len(s))

# 通过索引获取单个字符
print(s[0])
print(s[len(s) - 1])

# 布尔类型
b1 = True
b2 = False

# 空值类型
n = None

# type函数
print(type(s))
print(type(b1))
print(type(n))
print(type(1.5))

# 不能对布尔类型的变量使用len函数，因此下面一行会报错
# len(b1)
```

```python
# BMI = 体重 / (身高 ** 2)
user_weight = float(input("请输入您的体重（单位：kg）："))
user_height = float(input("请输入您的身高（单位：m）："))
user_BMI = user_weight / (user_height) ** 2
print("您的BMI值为：" + str(user_BMI))
```

```
mood_index = int(input("对象今天的心情指数是："))
if mood_index >= 60:
    print("恭喜，今晚应该可以打游戏，去吧皮卡丘！")
    print("∠( ᐛ 」∠)_")
else:  # mood_index < 60
    print("为了自个儿小命，还是别打了。")
```

```python
user_gender = input("请输入您的性别，M或F（M表示男，F表示女）：")
# BMI = 体重 / (身高 ** 2)
user_weight = float(input("请输入您的体重（单位：kg）："))
user_height = float(input("请输入您的身高（单位：m）："))
user_BMI = user_weight / user_height ** 2
print("您的BMI值为：" + str(user_BMI))

# 偏瘦：user_BMI <= 18.5
# 正常：18.5 < user_BMI <= 25
# 偏胖：25 < user_BMI <= 30
# 肥胖：user_BMI > 30
if user_BMI <= 18.5:
    if user_gender == "M":
        print("先生您好，此BMI值属于偏瘦范围。")
    elif user_gender == "F":
        print("女士您好，此BMI值属于偏瘦范围。")
    else:
        print("此BMI值属于偏瘦范围。")
elif 18.5 < user_BMI <= 25:
    if user_gender == "M":
        print("先生您好，此BMI值属于正常范围。")
    elif user_gender == "F":
        print("女士您好，此BMI值属于正常范围。")
    else:
        print("此BMI值属于正常范围。")
elif 25 < user_BMI <= 30:
    if user_gender == "M":
        print("先生您好，此BMI值属于偏胖范围。")
    elif user_gender == "F":
        print("女士您好，此BMI值属于偏胖范围。")
    else:
        print("此BMI值属于偏胖范围。")
else:
    if user_gender == "M":
        print("先生您好，此BMI值属于肥胖范围。")
    elif user_gender == "F":
        print("女士您好，此BMI值属于肥胖范围。")
    else:
        print("此BMI值属于肥胖范围。")
```

```python
shopping_list = []
# 往购物清单里添加两个商品
shopping_list.append("键盘")
shopping_list.append("键帽")
# 往购物清单里移除一个商品
shopping_list.remove("键帽")
# 往购物清单里移除两个商品
shopping_list.append("音响")
shopping_list.append("电竞椅")
# 更改购物清单的第二个商品
shopping_list[1] = "硬盘"

# print(shopping_list)
# print(len(shopping_list))
# print(shopping_list[0])

# 定义一个价格列表
price = [799, 1024, 200, 800]
# 获取最高的价格
max_price = max(price)
# 获取最低的价格
min_price = min(price)
# 获取从低到高排序好的价格列表
sorted_price = sorted(price)
print(max_price)
print(min_price)
print(sorted_price)
```

```python
# 结合input、字典、if判断，做一个查询流行语含义的电子词典程序
slang_dict = {"觉醒年代":"《觉醒年代》首次以电视剧的形式回溯中国共产党的孕育和创立过程，生动再现中国近代历史的大变局，深刻讲述中国人民是怎样选择了中国共产党。该剧播出后广受好评，成为党史学习教育的生动教材。",
              "YYDS":"“永远的神”的拼音缩写，用于表达对某人的高度敬佩和崇拜。2021年东京奥运会期间，不管是杨倩夺得首金，还是全红婵一场决赛跳出三个满分，或是“苏神”站上百米决赛跑道，全网齐喊“YYDS”，奥运期间一度刷屏。"}
slang_dict["双减"] = "指进一步减轻义务教育阶段学生作业负担和校外培训负担。其目标是使学校教育教学质量和服务水平进一步提升，作业布置更加科学合理，学校课后服务基本满足学生需要，学生学习更好回归校园，校外培训机构培训行为全面规范。"
slang_dict["破防"] = "原指在游戏中突破了对方的防御，使对方失去防御能力。现指因遇到一些事或看到一些信息后情感上受到很大冲击，内心深处被触动，心理防线被突破。"
slang_dict["元宇宙"] = "源于小说《雪崩》的科幻概念，现指在XR（扩展现实）、数字孪生、区块链和AI（人工智能）等技术推动下形成的虚实相融的互联网应用和社会生活形态。现阶段，元宇宙仍是一个不断演变、不断发展的概念。Facebook（脸书）对外公布更名为“Meta”，该词即来源于“Metaverse”（元宇宙）。"
slang_dict["绝绝子"] = "该词流行于某网络节目，节目中一些粉丝用“绝绝子”为选手加油。多用于赞美，表示“太绝了、太好了”。这个词引发了网友对网络语言的关注和讨论。"
slang_dict["躺平"] = "该词指人在面对压力时，内心再无波澜，主动放弃，不做任何反抗。“躺平”更像是年轻人的一种解压和调整方式，是改变不了环境便改变心态的自我解脱。短暂“躺平”是为了积聚能量，更好地重新出发。"
slang_dict["伤害性不高，侮辱性极强"] = "一段网络视频中，两名男子相互夹菜，而同桌的另一名女子则显得很孤单。于是有网友调侃“伤害性不高，侮辱性极强”。后被网友用来调侃某事虽然没有实质性危害，但是却令人很难堪。"
slang_dict["我看不懂，但我大受震撼"] = "源自导演李安在纪录片《打扰伯格曼》（2013）里评价一部影视作品的话。现多用于表示自己对某件事情的不解、震惊。"
slang_dict["强国有我"] = "源自建党百年天安门广场庆典上青年学子的庄严宣誓。“请党放心，强国有我”是青年一代对党和人民许下的庄重誓言，彰显着新时代中国青年的志气、骨气、底气。"

query = input("请输入您想要查询的流行语：")
if query in slang_dict:
    print("您查询的" + query + "含义如下")
    print(slang_dict[query])
else:
    print("您查询的流行语暂未收录。")
    print("当前本词典收录词条数为：" + str(len(slang_dict)) + "条。")
```

```python
print("哈喽呀！我是一个求平均值的程序。")
total = 0
count = 0
user_input = input("请输入数字（完成所有数字输入后，请输入q终止程序）：")
while user_input != "q":
    num = float(user_input)
    total += num
    count += 1
    user_input = input("请输入数字（完成所有数字输入后，请输入q终止程序）：")
if count == 0:
    result = 0
else:
    result = total / count
print("您输入的数字平均值为" + str(result))
```

```python
"""
写一个计算BMI的函数，函数名为 calculate_BMI。
1. 可以计算任意体重和身高的BMI值
2. 执行过程中打印一句话，"您的BMI分类为：xx"
3. 返回计算出的BMI值

BMI = 体重 / (身高 ** 2)

BMI分类
偏瘦：BMI <= 18.5
正常：18.5 < BMI <= 25
偏胖：25 < BMI <= 30
肥胖：BMI > 30
"""

def calculate_BMI(weight, height):
    BMI = weight / height ** 2
    if BMI <= 18.5:
        category = "偏瘦"
    elif BMI <= 25:
        category  = "正常"
    elif BMI <= 30:
        category = "偏胖"
    else:
        category = "肥胖"
    print(f"您的BMI分类为：{category}")
    return BMI

result = calculate_BMI(1.8, 70)
print(result)
```

