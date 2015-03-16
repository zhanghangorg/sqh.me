+++
Description = "在excel使手机号变为对应的手机邮箱"
Tags = ["excel","手机号","邮箱"]
date = "2011-05-06T16:47:17+08:00"
ds_title = "excle中把手机号判断为手机邮箱的公式"
title = "excle中把手机号判断为手机邮箱的公式"

+++
假设手机号码在c2单元格，，那么判断号码的公式如下：
```vba
=if(or(mid(c2,1,3)="134",mid(c2,1,3)="135",mid(c2,1,3)="136",mid(c2,1,3)="137",mid(c2,1,3)="138",mid(c2,1,3)="139",mid(c2,1,3)="187",mid(c2,1,3)="188",mid(c2,1,3)="150",mid(c2,1,3)="151",mid(c2,1,3)="152",mid(c2,1,3)="155",mid(c2,1,3)="157",mid(c2,1,3)="158",mid(c2,1,3)="159"),c2&amp;"@139.com",if(or(mid(c2,1,3)="130",mid(c2,1,3)="131",mid(c2,1,3)="132",mid(c2,1,3)="156",mid(c2,1,3)="185",mid(c2,1,3)="186"),c2&amp;"@wo.com.cn",if(or(mid(c2,1,3)="133",mid(c2,1,3)="153",mid(c2,1,3)="180",mid(c2,1,3)="189"),c2&amp;"@189.com","ERROR!")))
```