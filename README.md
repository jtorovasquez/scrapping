# scrapping
#installing a parser in python3
from urllib.request import urlopen
import html5lib

with urlopen(" http://py4e-data.dr-chuck.net/known_by_Fikret.htm") as f:
    document = html5lib.parse(f, transport_encoding=f.info().get_content_charset())
