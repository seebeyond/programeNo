# programeNo
验证性的
~~~
smp<-function(cross=fold_num,n,seed)
{
  set.seed(seed)
  dd=list()
  aa0=sample(rep(1:cross,ceiling(n/cross))[1:n],n)
  for (i in 1:cross) dd[[i]]=(1:n)[aa0==i]
  return(dd)
}
~~~
![image3](https://raw.githubusercontent.com/seebeyond/programeNo/master/image/Screenshot_2015-12-18-19-21-14.png)
