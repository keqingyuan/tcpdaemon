# 此文件由makeobj.sh自动生成
############################################################
# 项目名 : 
# 模块名 : 
# 备  注 : 
############################################################

###### 源文件配置区
#@ c_FILE
c_FILE		=	\
			test.c \
			testso.c \

###### 目标文件、安装目录配置区
NOINST_OBJ	=	testso.so test

###### 编译选项
CFLAGS		=	-I. \
			-I$(HOME)/exinc/tcpdaemon \

###### 链接选项
LFLAGS		=	-L. \
			-L$(HOME)/exlib \

###### 额外宏定义区
CLEAN_ADDITION	=

###### 加载mktpl模板库
#@ make_all
#@ make_clean
#@ make_install
#@ make_install_BININST
#@ make_install_DFTHDERINST

include $(MKTPLDIR)/makeobj_$(MKTPLOS).inc

###### 目标文件依赖关系
testso.so:	testso.o
	$(CC) $(SOFLAGS) -o $@ testso.o $(LFLAGS)

test	:	test.o
	$(CC) $(ESOFLAGS) -o $@ test.o $(LFLAGS) -ltcpdaemon

