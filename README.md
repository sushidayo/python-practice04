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
