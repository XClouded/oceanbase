# Copyright (C) 2004 MySQL AB
#
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 2 of the License, or
# (at your option) any later version.
# 
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
# 
# You should have received a copy of the GNU General Public License
# along with this program; if not, write to the Free Software
# Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA

noinst_LIBRARIES = libsboltp.a

libsboltp_a_SOURCES = sb_oltp.c ../sb_oltp.h

if USE_MYSQL

libsboltp_a_CPPFLAGS = -I$(srcdir)/.. $(AM_CPPFLAGS) $(MYSQL_CFLAGS) -I$(srcdir)/../../xmlconfig -I$(srcdir)/../../clientcommon -I./
#libsboltp_a_LIBFLAGS = -lsimon -L/home/xiaojun.chengxj/tools/ProjectObTest/sysbench-0.4.12/sysbench/clientcommon -lBasicsSubset -lsimon_sysbench -L/home/xiaojun.chengxj/tools/ProjectObTest/sysbench-0.4.12/sysbench/xmlconfig
else

libsboltp_a_CPPFLAGS = -I$(srcdir)/.. $(AM_CPPFLAGS)

endif

EXTRA_DIST = CMakeLists.txt
