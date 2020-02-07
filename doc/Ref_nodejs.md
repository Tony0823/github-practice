<style 
type="text/css">
h1 {color:black;}
p {color:black;}
.var-ch {color:red;}
.com-ch {color:#0000ff;}
.blk-ch {color:black;}
.markdown-body pre {
    padding: 10px;
    overflow: auto;
    font-size: 85%;
    line-height: 1.45;
    background-color: #ffffb0;
    border-radius: 3px;
}
</style>
# Node.js 문서 활용 예      

## Node.js

문서: <https://nodejs.org/ko/about/>

동영상:<https://www.inflearn.com/course/nodejs-%EA%B0%95%EC%A2%8C-%EC%83%9D%ED%99%9C%EC%BD%94%EB%94%A9/lecture/3510>

문서: <https://nodejs.org/ko/docs/>

### 사용 예


<https://nodejs.org/dist/latest-v12.x/docs/api/>

os 선택

<https://nodejs.org/dist/latest-v12.x/docs/api/os.html>

이 os모듈은 운영 체제 관련 유틸리티 방법 및 속성을 제공합니다. 다음을
사용하여 액세스 할 수 있습니다.



<span class= "var-ch">const</span> os = <span class= "com-ch">**require**</span>(\'os\');

[os.platform()](https://nodejs.org/dist/latest-v12.x/docs/api/os.html#os_os_platform)
선택

os.platform() &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\[[src](https://github.com/nodejs/node/blob/31d3b6d9cbf6f533e7990fa1b7f82976bc384c64/lib/os.js#L119)\]\#

Added in: v0.5.0`

Returns:
\<[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#String_type)\>

Returns a string identifying the operating system platform. The value is
set at compile time. Possible values are \'aix\', \'darwin\',
\'freebsd\', \'linux\', \'openbsd\', \'sunos\', and \'win32\'.

운영 체제 플랫폼을 식별하는 문자열을 반환합니다. 이 값은 컴파일 타임에
설정됩니다. 가능한 값은 \'aix\', \'darwin\', \'freebsd\', \'linux\',
\'openbsd\', \'sunos\',와 \'win32\'.

The return value is equivalent to
[process.platform](https://nodejs.org/dist/latest-v12.x/docs/api/process.html#process_process_platform).

The value \'android\' may also be returned if Node.js is built on the
Android operating system. [Android support is
experimental.](https://github.com/nodejs/node/blob/master/BUILDING.md#androidandroid-based-devices-eg-firefox-os)

\'android\'Node.js가 Android 운영 체제에서 빌드 된 경우에도 값 이 리턴
될 수 있습니다. 안드로이드 지원은 실험적이다.

File을 하나 만든다.   
 예) moudule.js

moudule.js:   
<pre><code><span class= "var-ch">var</span> o = <span class= "com-ch">require</span><span class="blk-ch">(\'os\');</span>
<span class="blk-ch">console.log(o.platform());</span></code></pre>

   
터미날에서
<pre><span class="blk-ch"> node module.js</span></pre>  

window에서는 아래와 같이 win32가 표시된다

C:\\Work\_js\\server\_side\_javascript\_tutorials-master\>node module.js

win32
