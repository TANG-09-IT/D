from PIL import Image

# 初始化result变量
result = None

# 计算器逻辑（后续代码不变）
num1 = float(input("请输入第一个数："))
op = input("请输入运算符(+、-、*、/)：")
num2 = float(input("请输入第二个数："))

if op == '+':
    result = num1 + num2
elif op == '-':
    result = num1 - num2
elif op == '*':
    result = num1 * num2
elif op == '/':
    if num2 != 0:
        result = num1 / num2
    else:
        print("除数不能为0")
else:
    print("输入的符号无效")

if result is not None:
    print(f"结果：{result}")

# 图片处理逻辑
img = Image.open(r'C:\Users\唐俊杰\Desktop\pcoek.jpg')
img.show()
