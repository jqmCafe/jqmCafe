
<!--

```Rust
#![no_std] // Minimal kernel
#![no_main]
use core::panic::PanicInfo;
#[panic_handler]
fn panic(_info: &PanicInfo) -> ! { loop {} }
#[no_mangle]
pub extern "C" fn _start() -> ! {
    let message = "Hi, I am Stardust!"; // ☬
    let buffer = 0xb8000 as *mut u8;
    for (i, &b) in message.as_bytes().iter().enumerate() {
        unsafe { // ☈
            *buffer.offset(i as isize * 2) = b;
            *buffer.offset(i as isize * 2 + 1) = 0xb;
        }
    }
    loop {}
}
``` 


<img alt="GitHub followers" src="https://img.shields.io/github/followers/jqmCafe?style=flat-square&logo=github" /> 


# ❀ Website ❀
[![Stardust Preview](https://hanabi-ai.cn/preview.png)](https://hanabi-ai.cn)



# 📞 ❅ Contact ❅

```text
Email: stardust@fish.audio
Bilibili: @Stardust_减
Github: @Stardust-minus
QQ:2225664821
```

https://raw.githubusercontent.com/innng/innng/master/assets/kyubey.gif
-->

# ஐ coffee ஐ 

<img align="right" width="400" src="https://github.com/AlldDev/AlldDev/blob/main/assets/bg.gif" />

```Python
def main():
    message = "Hi, I am Café!"
    # \033[36m = ciano, \033[0m = reset
    print("\033[36m" + message + "\033[0m")

if __name__ == "__main__":
    main()

```

# 〄 Analysis 〄

<img width="44%" align="left" src="https://github-readme-stats.vercel.app/api?username=jqmCafe&count_private=true&show_icons=true&theme=radical" />
<img width="50%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=jqmCafe&theme=radical" />
