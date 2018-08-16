# HelperBox
#### 이 repository는 IAMROOT15A 팀이 개발 및 분석에 필요한 Tool, Script, Configuration 등을 공유하기 위한 repository입니다.

1. mkcscope.sh
1.1 chmod +x mkcscope.sh

1.2 cp mkcscope.sh /usr/bin/mkcscope

1.3 Insert below script in .vimrc

"cscope

set csprg=/usr/bin/cscope
set csto=0
set cst
set nocsverb

if filereadable("./cscope.out")
	cs add cscope.out
else
	cs add /usr/src/linux/cscope.out
endif
set csverb
"cscope

