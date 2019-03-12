# GCC 컴파일러
gcc설치 확인을 위해 -m32 -m64 옵션을 사용해 보았더니 test32실행파일이 만들어지지 않았다.  
알고보니 기존 우분투 18.04LTS에 설치된 gcc가 -m 옵션을 지원하지 않아 삽질하다 겨우 패키지를 찾았다ㅠㅠ.
<pre><code>sudo apt-get install gcc-multilib</code></pre>
위 패키지를 설치하여 해결했다.