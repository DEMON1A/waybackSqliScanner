# waybackSqliScanner
- Modifed Version Of waybackSqliScanner With New Update That Fixes The Bytes Error And Colored Output.

## Why I Created This?
- The Author Of waybackSqliScanner Is Inactive For 1 Year. And Some People Pointed Some Issue About That The Program Doesn't Work 2 Years Ago, There's Was An Error On The Code That Stopped The Scanning Process But The Threading Disallowed Showing Python Errors. I Fixed The Issue And Posted The Details On [Comment](https://github.com/ghostlulzhacks/waybackSqliScanner/issues/2#issuecomment-774298233) But I Think It Won't Be Any Action From The Author. So I Created a New Version On It And Made Few Changes To The Code. The Code Belongs To The Author. It's Not Mine. I'm Just Posting an Update For This Case.

## Install And Use It:
```
git clone https://github.com/DEMON1A/waybackSqliScanner
cd waybackSqliScanner/
python3 main.py [DOMAIN]/[FILE_PATH]
```

## Wanna Test It? - Where Were The Error?
- You Can Test It Out On `testphp.vulnweb.com` With This Command: `python3 main.py testphp.vulnweb.com`. That Verifies The Tool Is Working After The Update. The Error Was On Line *48* The Author Was Using The Response Content as Bytes With `.content` But Regex Is Using String Compare. So The Fix Was To Change `html = r.content` Into `html = r.text`
