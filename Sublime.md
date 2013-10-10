
###快捷键
1. cmd+T 快速查找文件
2. cmd+R 列出当前类的方法


###辅助使用
1.建立软连接，使sublime可以从shell中启动
```sh
sudo ln -s /Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl /usr/bin/subl

现在就可以使用`subl .`打开当前文件夹
```
2.安装package control

1. ctrl+`
2. 输入
```sh
import urllib2,os; pf='Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler( ))); open( os.path.join( ipp, pf), 'wb' ).write( urllib2.urlopen( 'http://sublime.wbond.net/' +pf.replace( ' ','%20' )).read()); print( 'Please restart Sublime Text to finish installation')
```
3. cmd+shift+p,输入 install package 就可以安装插件了

#####推荐插件
1. gitgutter
