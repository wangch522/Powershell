
```Restart-Computer -whatif   whatif是告诉你命令是做什么```

##操作符
    -like
    -match
    -eq 
    -Cmatch (严格区分大小写)
    -le
    -lt

| ft autosize, 格式化字段输出全部字符

Get-Member 获取属性和方法
$var| Get-Member

Get-Services [1] | Select-object  获取更具体的属性