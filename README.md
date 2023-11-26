# sdl2-setup
najprej downloadate SDL file iz https://github.com/libsdl-org/SDL/releases/tag/release-2.28.5

![SDL file](https://github.com/CrushedCookieNut/sdl2-setup/assets/96495881/73e0f83d-c36b-4ee0-beb0-36c410e4a62a)

nato ga extractate, lahko v project folder ali pa tudi drugam

nato iz tega kar ste dobili greste v i686-w64-mingw32 ali x86_64-w64-mingw32, odvisno ali imate 64 ali 32 bitni sistem in v svoj project folder kopirate include in lib mapo ter SDL2.dll iz mape bin

nato kopirate moj main.cpp ali naredite svojega in MakeFile

če vam vrže error zaradi #include <SDL2/SDL.h>, potem držite miško nad includeom ter kliknite na QuickFix in prvo opcijo oz. repair includePath, popravilo se bo samo

samo prepirčajte se, da izgleda potem tako


![includePath](https://github.com/CrushedCookieNut/sdl2-setup/assets/96495881/7c499387-804b-474c-973c-9947aaac22d4)

če vam ukaz v MakeFileu ne deluje, ker nimate mingw compilerja, uporabite to: g++ -I src/include -L src/lib -o main main.cpp -lSDL2main -lSDL2

če pa vam MakeFile sploh ne deluje, lahko to komando vpišete direktno v terminal

vaš project folder zdaj izgleda tako:


![project folder](https://github.com/CrushedCookieNut/sdl2-setup/assets/96495881/7bc56788-74fd-4524-87a2-d1523a07d7d6)

sedaj v terminal samo še napišite ./main in, če se vam odpre okno ste vse naredili prav
