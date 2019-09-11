# if 的嵌套

```python
ticket = int(input("输入是否购票")) # 1表示有车票 0表示没有车票

kn = int(input("输入刀子长度")) # cm

# 先判断是否有车票
if ticket == 1:
    print("通过了车票检查，可以进站")
    # 判断刀的长度
    if kn <= 10:
        print("通过安检，可以乘车")
    else:
        print("安检没有通过")
else:
    print("没车票")
```

