Pluot
=====

A tiny language that compiles into C

Pluot is C with a Python-like syntax. 

Pluot frees you from semicolon-itis by assigning meaning to newlines:

<code><pre>int i = 0

printf("Hello there.\n")

unleash(penguins)</pre></code>

becomes

<code><pre>int i = 0;

printf("Hello there.\n");

unleash(penguins);</pre></code>

Pluot eliminates C's curly braces with a cleaner, Python-style indentation:

<code><pre>int i = 0
while ++i < 10
    if radiationInTankNo(i)
        printf("Plutonium found in tank number %d.\n", i)</pre></code>

<code><pre>int i = 0;
while (++i &lt; 10)
{
    if (radiationInTankNo(i))
    {
        printf("Plutonium found in tank number %d.\n", i);
    }
}</pre></code>

Pluot uses the power of the English language to make your code more readable by allowing you to use English operators and constructs.

<code><pre>int unacceptable(int j)
    return j is 18 or j % 2 is 0

void main()
    int i = 1

    until ++i >= 100
        unless unacceptable(i)
            printf("%d\n", i)
        else
            printf("No way.\n")</pre></code>

<code><pre>
int unacceptable(int j)
{
    return j == 18 || j % 2 == 0;
}

int i = 1;

void main()
{
    while (!(100 &gt;= ++i))
    {
        if (! unacceptable(i))
        {
            printf("%d\n", i);
        }
        else 
        {
            printf("No way.\n");
        }
    }
}</pre></code>


