# python-practice04

import re
s = 'Learn Python'

mobj = re.match('Le',s)
if mobj:
    print(mobj.group() )
    
mobj = re.search('Py', s)

import re
s = 'Learn Python'
reobj = re.compile('Le')
mobj = reobj.match(s)
if mobj:
    print(mobj.group() )
    
mobj = re.match('Le', s,re.IGNORECASE)
reobj = re.compile('Le', re.IGNORECASE)
print(mobj)
print(reobj)

import re
s = 'Learn Python'
mlist = re.findall('.n', s)

re.match('L.*n', 'Learn Python').group()
print(s)

import re
s = 'Learn Python'
miter = re.finditer('.n', s)
for mobj in miter:
    print(mobj.group() )
    print(mobj.span() )

import re
s1 = 'Python Fang'
s2 =re.sub('[A-Z].{2]', 'e', s1)
print(s1)

import re
s = 'Learn Python, Shiori'
mlist = re.split('.n', s)
print(s)

import re
s = 'Learn Python, Shiori'
mobj = re.match('Le', s)
print(s)
