- 👋 Hi, I’m @Trien2k5
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Trien2k5/Trien2k5 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#include <iostream>
#include <thread>
#include <chrono>
#include <vector>

// Hàm để in cây thông Năm Mới
void printNewYearTree() {
    std::vector<std::string> tree = {
        "       *       ",
        "      ***      ",
        "     *****     ",
        "    *******    ",
        "   *********   ",
        "  ***********  ",
        " ************* ",
        "***************",
        "      ***      "
    };

    for (const auto &line : tree) {
        std::cout << line << std::endl;
        std::this_thread::sleep_for(std::chrono::milliseconds(300));
    }
}

// Hàm để in thông điệp chúc mừng Năm Mới
void printHappyNewYear() {
    std::string message = R"(
 _    _                     _  __     __  _             
| |  | |                   | | \ \   / / | |            
| |  | |  _   _   _ __     | |  \ \_/ /  | |            
| |  | | | | | | | '_ \    | |   \   /   | |            
| |__| | | |_| | | | | |   | |    | |    | |____        
 \____/   \__,_| |_| |_|   |_|    |_|    |______|       
                                                     
    )";
    std::cout << message << std::endl;
    std::this_thread::sleep_for(std::chrono::seconds(1));
}

// Hàm để in pháo hoa
void printFireworks() {
    std::vector<std::string> fireworks = {
        "            .        +          .      .          .        .        .      ",
        "     .         ____     .      .   .      +          .         .        . ",
        "   .        .-'    `-.      .    .    .       .  .        .  +    .      .",
        "       +  .'          `. .    .     .   . .       .  .   .      .   .     ",
        "          /   .-''''-.   \   .   .  +    .       .    .  .    .     .    .",
        "  .      /   /        \   \       .   .     .  .     .   .    .  +    .  .",
        "        |   |          |   | .    .     +       .   .  .    .  .   .      ",
        " .       \   \        /   /    .    .  .    .    .     .     .       .    ",
        "  +       '.  `-....-'  .'       .   .  +    .      .  .  +    .   .    . ",
        "     .     `.        .'    .  .      .     .  .    .    .     .  .     .  ",
        "  .          `-....-'       .    .      + .    .     +    .  .      +     ",
    };

    for (const auto &line : fireworks) {
        std::cout << line << std::endl;
        std::this_thread::sleep_for(std::chrono::milliseconds(200));
    }
}

int main() {
    printNewYearTree();
    printHappyNewYear();
    printFireworks();
    return 0;
}
