# Preparing the Docker Containers

In order to run the challenge POCs without any problem, I prepared docker containers for various Ubuntu releases. The instructions for using the containers can be found [here](docker).

# Writeups

| CTF                        | Challenge   | Info               | Exploitation         | Links     |
|:--------------------------:|:-----------:|--------------------|----------------------|:---------:|
| [UTCTF 2019](UTCTF/2019)| [babyecho](UTCTF/2019/babyecho) | `x86_32`<br>`NX`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`format string`<br>`libc database` | [CTFtime](https://ctftime.org/event/757)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/UTCTF/2019) |
| [BSidesSF 2019](BSidesSF/2019)| [slowfire](BSidesSF/2019/slowfire) | `x86_64`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`PLT`<br>`shellcode`<br>`socket`<br>`stack overflow`<br>`syscall` | [CTFtime](https://ctftime.org/event/753)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/BSidesSF/2019) |
| [TAMUctf 2019](TAMUctf/2019)| [pwn3](TAMUctf/2019/pwn3) | `x86_32`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `shellcode`<br>`stack overflow`<br>`syscall` | [CTFtime](https://ctftime.org/event/740)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/TAMUctf/2019) |
| [TAMUctf 2019](TAMUctf/2019)| [pwn5](TAMUctf/2019/pwn5) | `x86_32`<br>`NX`<br>`Partial RELRO`<br>`ASLR` | `ret2libc`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/740)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/TAMUctf/2019) |
| [ASIS 2018 Finals](ASIS/2018/Finals)| [asvdb](ASIS/2018/Finals/asvdb) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`ASLR` | `__free_hook`<br>`double free`<br>`heap`<br>`one gadget`<br>`smallbin`<br>`tcache dup`<br>`tcache poisoning`<br>`tcache`<br>`unsorted bin`<br>`use after free` | [CTFtime](https://ctftime.org/event/620)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/ASIS/2018/Finals) |
| [ASIS 2018 Finals](ASIS/2018/Finals)| [inception](ASIS/2018/Finals/inception) | `x86_64`<br>`NX`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`ROP`<br>`fork`<br>`one gadget`<br>`pipe`<br>`return-to-csu`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/620)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/ASIS/2018/Finals) |
| [SECCON 2018 Quals](SECCON/2018/Quals)| [profile](SECCON/2018/Quals/profile) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `C++`<br>`GOT`<br>`arbitrary read`<br>`buffer overflow`<br>`one gadget`<br>`string` | [CTFtime](https://ctftime.org/event/683)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/SECCON/2018/Quals) |
| [SECCON 2018 Quals](SECCON/2018/Quals)| [classic](SECCON/2018/Quals/classic) | `x86_64`<br>`NX`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`ROP`<br>`one gadget`<br>`stack overflow`<br>`stack pivoting` | [CTFtime](https://ctftime.org/event/683)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/SECCON/2018/Quals) |
| [BSidesDelhi 2018](BSidesDelhi/2018)| [data_bank](BSidesDelhi/2018/data_bank) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `__malloc_hook`<br>`heap`<br>`one gadget`<br>`tcache poisoning`<br>`tcache`<br>`use after free` | [CTFtime](https://ctftime.org/event/700)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/BSidesDelhi/2018) |
| [HITCON 2018](HITCON/2018)| [children_tcache](HITCON/2018/children_tcache) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `__malloc_hook`<br>`double free`<br>`heap`<br>`off-by-one`<br>`overlapping chunks`<br>`poison-null-byte`<br>`tcache dup`<br>`tcache poisoning`<br>`tcache` | [CTFtime](https://ctftime.org/event/669)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/HITCON/2018) |
| [Hack.lu 2018](Hack.lu/2018)| [babyphp](Hack.lu/2018/babyphp) | `Web`<br>`PHP` | `assert`<br>`code injection`<br>`unintended behaviors`<br>`unsanitized input` | [CTFtime](https://ctftime.org/event/699)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/Hack.lu/2018) |
| [InCTF 2018](InCTF/2018)| [warmup](InCTF/2018/warmup) | `arm`<br>`arm32`<br>`armhf`<br>`Partial RELRO`<br>`ASLR` | `shellcode`<br>`stack overflow`<br>`syscall` | [CTFtime](https://ctftime.org/event/662)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/InCTF/2018) |
| [InCTF 2018](InCTF/2018)| [yawn](InCTF/2018/yawn) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`ASLR` | `GOT`<br>`__malloc_hook`<br>`fastbin dup`<br>`heap`<br>`off-by-one`<br>`one gadget` | [CTFtime](https://ctftime.org/event/662)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/InCTF/2018) |
| [InCTF 2018](InCTF/2018)| [securepad](InCTF/2018/securepad) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `__free_hook`<br>`arbitrary free`<br>`fastbin dup`<br>`heap`<br>`uninitialized var`<br>`unsorted bin` | [CTFtime](https://ctftime.org/event/662)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/InCTF/2018) |
| [CSAW 2018 Quals](CSAW/2018/Quals)| [alien_invasion](CSAW/2018/Quals/alien_invasion) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`PIE`<br>`ASLR` | `GOT`<br>`heap`<br>`off-by-one`<br>`overlapping chunks`<br>`poison-null-byte` | [CTFtime](https://ctftime.org/event/633)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/CSAW/2018/Quals) |
| [CSAW 2018 Quals](CSAW/2018/Quals)| [bigboy](CSAW/2018/Quals/bigboy) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `stack overflow` | [CTFtime](https://ctftime.org/event/633)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/CSAW/2018/Quals) |
| [CSAW 2018 Quals](CSAW/2018/Quals)| [get_it](CSAW/2018/Quals/get_it) | `x86_64`<br>`NX`<br>`Partial RELRO`<br>`ASLR` | `stack overflow` | [CTFtime](https://ctftime.org/event/633)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/CSAW/2018/Quals) |
| [CSAW 2018 Quals](CSAW/2018/Quals)| [shell_code](CSAW/2018/Quals/shell_code) | `x86_64`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `shellcode`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/633)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/CSAW/2018/Quals) |
| [WhiteHat 2018 Quals](WhiteHat/2018/Quals)| [pwn02](WhiteHat/2018/Quals/pwn02) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`FORTIFY`<br>`ASLR` | `glibc tcache`<br>`heap`<br>`off-by-one`<br>`overlapping chunks`<br>`poison-null-byte` | [CTFtime](https://ctftime.org/event/656)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/WhiteHat/2018/Quals) |
| [MeePwn 2018 Quals](MeePwn/2018/Quals)| [babysandbox](MeePwn/2018/Quals/babysandbox) | `x86_32`<br>`NX`<br>`Partial RELRO`<br>`PIE`<br>`ASLR` | `openat`<br>`readv`<br>`shellcode`<br>`socket`<br>`syscall`<br>`writev` | [CTFtime](https://ctftime.org/event/625)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/MeePwn/2018/Quals) |
| [0CTF 2018 Finals](0CTF/2018/Finals)| [freenote2018](0CTF/2018/Finals/freenote2018) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `__malloc_hook`<br>`double free`<br>`fastbin dup`<br>`heap metadata`<br>`heap`<br>`overlapping chunks` | [CTFtime](https://ctftime.org/event/558)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/0CTF/2018/Finals) |
| [RCTF 2018](RCTF/2018)| [rnote3](RCTF/2018/rnote3) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `__free_hook`<br>`fastbin`<br>`heap`<br>`one gadget`<br>`overlapping chunks`<br>`uninitialized var` | [CTFtime](https://ctftime.org/event/624)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/RCTF/2018) |
| [RCTF 2018](RCTF/2018)| [babyheap](RCTF/2018/babyheap) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `PREV_IN_USE bit`<br>`__malloc_hook`<br>`heap`<br>`off-by-one`<br>`poison-null-byte` | [CTFtime](https://ctftime.org/event/624)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/RCTF/2018) |
| [RCTF 2018](RCTF/2018)| [stringer](RCTF/2018/stringer) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `IS_MMAPED`<br>`__malloc_hook`<br>`calloc`<br>`double free`<br>`fastbin dup`<br>`heap`<br>`off-by-one` | [CTFtime](https://ctftime.org/event/624)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/RCTF/2018) |
| [PlaidCTF 2018](PlaidCTF/2018)| [shop](PlaidCTF/2018/shop) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`buffer overflow`<br>`heap`<br>`one gadget` | [CTFtime](https://ctftime.org/event/617)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/PlaidCTF/2018) |
| [ASIS 2018 Quals](ASIS/2018/Quals)| [cat](ASIS/2018/Quals/cat) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`fastbin`<br>`heap` | [CTFtime](https://ctftime.org/event/568)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/ASIS/2018/Quals) |
| [ASIS 2018 Quals](ASIS/2018/Quals)| [fifty_dollars](ASIS/2018/Quals/fifty_dollars) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `double free`<br>`fastbin`<br>`heap`<br>`use after free` | [CTFtime](https://ctftime.org/event/568)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/ASIS/2018/Quals) |
| [ASIS 2018 Quals](ASIS/2018/Quals)| [just_sort](ASIS/2018/Quals/just_sort) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`heap overflow`<br>`one gadget` | [CTFtime](https://ctftime.org/event/568)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/ASIS/2018/Quals) |
| [ASIS 2018 Quals](ASIS/2018/Quals)| [message_me](ASIS/2018/Quals/message_me) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `__malloc_hook`<br>`double free`<br>`fastbins`<br>`heap`<br>`overlapping chunks`<br>`use after free` | [CTFtime](https://ctftime.org/event/568)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/ASIS/2018/Quals) |
| [StarCTF 2018](StarCTF/2018)| [babystack](StarCTF/2018/babystack) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`ASLR` | `GOT`<br>`pthread`<br>`stack overflow`<br>`stack_guard`<br>`thread local storage` | [CTFtime](https://ctftime.org/event/614/)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/StarCTF/2018) |
| [StarCTF 2018](StarCTF/2018)| [note](StarCTF/2018/note) | `x86_64`<br>`NX`<br>`Full RELRO`<br>`ASLR` | `GOT`<br>`LSB`<br>`ROP`<br>`off-by-one`<br>`saved rbp`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/614/)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/StarCTF/2018) |
| [StarCTF 2018](StarCTF/2018)| [warmup](StarCTF/2018/warmup) | `x86_64`<br>`NX`<br>`Full RELRO`<br>`ASLR` | `GOT`<br>`one gadget`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/614/)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/StarCTF/2018) |
| [WPICTF 2018](WPICTF/2018)| [forker.level1](WPICTF/2018/forker.level1) | `x86_64`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`ROP`<br>`return-to-csu`<br>`shellcode`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/600)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/WPICTF/2018) |
| [WPICTF 2018](WPICTF/2018)| [forker.level2](WPICTF/2018/forker.level2) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `fork`<br>`socket`<br>`stack canary`<br>`stack cookie`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/600)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/WPICTF/2018) |
| [UIUCTF 2018](UIUCTF/2018)| [how2heap](UIUCTF/2018/how2heap) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `heap`<br>`one gadget` | [CTFtime](https://ctftime.org/event/587)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/UIUCTF/2018) |
| [0CTF 2018 Quals](0CTF/2018/Quals)| [babyheap](0CTF/2018/Quals/babyheap) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `__malloc_hook`<br>`double free`<br>`fastbin dup`<br>`heap`<br>`off-by-one`<br>`one gadget`<br>`top chunk` | [CTFtime](https://ctftime.org/event/557)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/0CTF/2018/Quals) |
| [0CTF 2018 Quals](0CTF/2018/Quals)| [babystack](0CTF/2018/Quals/babystack) | `x86_32`<br>`NX`<br>`Partial RELRO`<br>`ASLR` | `Elf_Rel`<br>`Elf_Sym`<br>`GOT`<br>`PLT`<br>`ROP`<br>`dynstr`<br>`dynsym`<br>`rel_plt`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/557)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/0CTF/2018/Quals) |
| [iCTF 2018](iCTF/2018)| [fantasticiot](iCTF/2018/fantasticiot) | `x86_32`<br>`NX`<br>`Canary`<br>`ASLR` | `attack & defense`<br>`binary patching`<br>`strncmp` | [CTFtime](https://ctftime.org/event/567)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/iCTF/2018) |
| [TAMUctf 2018](TAMUctf/2018)| [pwn5](TAMUctf/2018/pwn5) | `x86_32`<br>`NX`<br>`Partial RELRO`<br>`ASLR` | `ROP`<br>`stack overflow`<br>`syscall` | [CTFtime](https://ctftime.org/event/559)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/TAMUctf/2018) |
| [NullconHackIM 2018](NullconHackIM/2018)| [pwn2-box](NullconHackIM/2018/pwn2-box) | `x86_64`<br>`Partial RELRO`<br>`ASLR` | `ROP`<br>`one gadget`<br>`shellcode`<br>`syscall` | [CTFtime](https://ctftime.org/event/566)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/NullconHackIM/2018) |
| [Codegate 2018 Quals](Codegate/2018/Quals)| [baskin_robins31](Codegate/2018/Quals/baskin_robins31) | `x86_64`<br>`NX`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`ROP`<br>`one gadget`<br>`stack overflow`<br>`stack pivot` | [CTFtime](https://ctftime.org/event/542)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/Codegate/2018/Quals) |
| [Codegate 2018 Quals](Codegate/2018/Quals)| [super_marimo](Codegate/2018/Quals/super_marimo) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`fastbin`<br>`heap`<br>`one gadget` | [CTFtime](https://ctftime.org/event/542)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/Codegate/2018/Quals) |
| [0CTF 2017 Quals](0CTF/2017/Quals)| [babyheap](0CTF/2017/Quals/babyheap) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `IS_MMAPED`<br>`__malloc_hook`<br>`calloc`<br>`fastbin attack`<br>`fastbin`<br>`heap overflow`<br>`one gadget`<br>`smallbin` | [CTFtime](https://ctftime.org/event/402)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/0CTF/2017/Quals) |
| [C3CTF 2017](C3CTF/2017)| [simplegc](C3CTF/2017/simplegc) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`fastbin`<br>`glibc tcache`<br>`heap`<br>`use after free` | [CTFtime](https://ctftime.org/event/544)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/C3CTF/2017) |
| [SECCON 2017 Quals](SECCON/2017/Quals)| [election](SECCON/2017/Quals/election) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`ASLR` | `GOT`<br>`__malloc_hook`<br>`fastbin`<br>`null byte overflow`<br>`null byte poisoning`<br>`off-by-one`<br>`one gadget` | [CTFtime](https://ctftime.org/event/512)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/SECCON/2017/Quals) |
| [SECCON 2017 Quals](SECCON/2017/Quals)| [secure_keymanager](SECCON/2017/Quals/secure_keymanager) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`PLT`<br>`double free`<br>`fastbin`<br>`format string`<br>`heap` | [CTFtime](https://ctftime.org/event/512)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/SECCON/2017/Quals) |
| [SECCON 2017 Quals](SECCON/2017/Quals)| [video_player](SECCON/2017/Quals/video_player) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `GOT`<br>`__malloc_hook`<br>`fastbin`<br>`heap`<br>`one gadget`<br>`overlapping chunks`<br>`use after free`<br>`virtual calls`<br>`vtable` | [CTFtime](https://ctftime.org/event/512)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/SECCON/2017/Quals) |
| [CSAW 2017 Quals](CSAW/2017/Quals)| [scv](CSAW/2017/Quals/scv) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `ROP`<br>`buffer over-read`<br>`buffer overflow`<br>`information disclosure`<br>`one gadget`<br>`stack overflow` | [CTFtime](https://ctftime.org/event/488)<br>[CTFium](https://github.com/sajjadium/CTFium/tree/master/CSAW/2017/Quals) |
