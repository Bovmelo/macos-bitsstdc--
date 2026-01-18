Run the following command to build the stdc++.h file for your macOS:

```sh
curl -fsSL https://raw.githubusercontent.com/Bovmelo/macos-bitsstdc--/refs/heads/main/build.sh | sudo zsh
```

Then, enjoy including `bits/stdc++.h` in your code!

The stdc++.h is a subset of the bits/stdc++.h file from the 15.2.0 GNU C++ Library, and it's compatible with the Apple Clang.


----

想在 MacOS 上使用 bits/stdc++.h？

Wanna use bits/stdc++.h on MacOS?

众所周知，MacOS 中的 g++ 命令是 Apple Clang．尽管从 Homebrew 等地方可以安装 GNU GCC，然而其他调试功能，如 sanitizer（-fsanitize=address 等）， GNU GCC 需要配套 GNU 的 libasan / libubsan 等运行时库，而 MacOS 作为一个封闭的操作系统显然并不被认真对待．

As you may know, the g++ command on MacOS actually uses Apple Clang. While you can install GNU GCC through Homebrew and other sources, using features like sanitizers (e.g., -fsanitize=address) with GCC requires runtime libraries such as libasan and libubsan. Unfortunately, since MacOS is a closed operating system, support for these is limited and often overlooked.

但是 Apple Clang 在竞赛编程等简单的应用场景中，与 GNU GCC 相比，并没有什么致命的差别，除了用不了 `bits/stdc++.h`．

However, in some lightweight scenarios like competitive programming, there is no significant difference between Apple Clang and GNU GCC, except for, `bits/stdc++.h`．

如果这个仓库对你有帮助，请点一个不要钱的小星星吧 sto

If this repository has been helpful for you, please consider leaving a free star :)
