# learn-c-
1 2 3 // this code won't compile! enum Color {RED, GREEN, BLUE};  enum Feelings {EXCITED, MOODY, BLUE};
1
2
3
4
5
Color color = Color::GREEN;
if ( Color::RED == color )
{
    // the color is red
}
1
2
3
4
5
6
enum class Mood;
 
void assessMood (Mood m);
  
// later on:
enum class Mood { EXCITED, MOODY, BLUE };
1
2
// we only have three colors, so no need for ints!
enum class Colors : char { RED = 1, GREEN = 2, BLUE = 3 };
1
2
#include <cstdint>
enum class Colors : std::int8_t { RED = 1, GREEN = 2, BLUE = 3 };
1
2
3
4
void func(int n); 
void func(char *s);
 
func( NULL ); // guess which function gets called?
std::nullptr_t
1
decltype( nullptr )
1
std::nullptr_t
1
void func( std::nullptr_t );
