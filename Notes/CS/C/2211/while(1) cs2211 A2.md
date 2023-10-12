

while(1) {  // 在[[C语言]]中[[while(1) cs2211 A2]] 代表一个永远不会结束的循环，除非内部有break语句或其他退出机制
        printf("请输入一个非负指数（输入0退出）：");
        scanf("%u", &exponent);

        if (exponent == 0) {
            printf("2^0 = 1\n");
            printf("退出程序...\n");
            break;  // 当用户输入0时，使用break退出while循环，结束程序
        }

        printf("2^%u = %lu\n\n", exponent, powerOfTwo(exponent));
    }
