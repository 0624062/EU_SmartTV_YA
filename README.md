```java
abstract class  CShape
{
    protected String color;
    public void setColor(String str)
    {
        color = str;
    }
    public abstract void show();
}
class CTriangle extends CShape
{
    protected double a, b, c;
    public CTriangle(double a, double b, double c)
    {
        a = a;
        b = b;
        c = c;
    }
    public void show()
    {
        System.out.print("color="+color+", ");
        System.out.print("area="+0.5*a*b);
    }
}
public class Main{
    public static void main(String args[]){
        CTriangle CTriangle = new CTriangle(3,4,5);
        CTriangle.setColor("Red");
        CTriangle.show();
    }
 }

```
