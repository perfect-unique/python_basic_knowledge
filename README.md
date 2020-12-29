## Python 练习册，每天一个小程序 ##
**第一题**求一个数中数字的和:
def main():
    while True:
        a = int(input("任意输入一个数:"))
        sum = 0
        for i in range(len(a)):
            sum = sum + int(a[i])
        print('{}'.format(sum))

if __name__ == '__main__':
    main()
**第二题**在列表中按规定去除重复的内容：
def main():
    list = [1, 2, 1, 2, 1, 1, 1]
    for i in list[::]:    #切片
        if i == 1:  #去除重复出现的1或者可以list1 = [i for i in list if i != 1]
            list.remove(i)
	    #list1 = set（list）#去除重复出现的项。
    print(list)
if __name__ == '__main__':
    main()
