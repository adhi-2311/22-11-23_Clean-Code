## review 1
Given :<code>
public bool IsShopOpen(string day)
{
    if (!string.IsNullOrEmpty(day))
    {
        day = day.ToLower();
        if (day == "friday")
        {
            return true;
        }
        else if (day == "saturday")
        {
            return true;
        }
        else if (day == "sunday")
        {
            return true;
        }
        else
        {
            return false;
        }
    }
    else
    {
        return false;
    }

}
</code>
Expected: 
<code>
public bool IsShopOpen(string day)
{
    if (string.IsNullOrEmpty(day))
    {
        return false;
    }
    var openingDays=new[]{"friday","saturday","sunday"};
    return openingDays.Any(d=>d==day.ToLower());
}
</code>
<hr></hr>

## review 3
Given:
<code>public long Fibonacci(int n)
{
    if (n < 50)
    {
        if (n != 0)
        {
            if (n != 1)
            {
                return Fibonacci(n - 1) + Fibonacci(n - 2);
            }
            else
            {
                return 1;
            }
        }
        else
        {
            return 0;
        }
    }
    else
    {
        throw new System.Exception("Not supported");
    }
}</code>
Expected: <code>public long Fibonacci(int n)
{
    if (n < 50)
    {
       if(n>1)
       return Fibonacci(n-1)+Fibonacci(n-2);
       else
       return n;
    }
    else
    {
        throw new System.Exception("Not supported");
    }
}</code>
<hr></hr>

## review 4
Given: <code>var l = new[] { "Austin", "New York", "San Francisco" };

for (var i = 0; i < l.Count(); i++)
{
    var li = l[i];
    DoStuff();
    DoSomeOtherStuff();

    // ...
    // ...
    // ...
    // Wait, what is `li` for again?
    Dispatch(li);
}</code>

Expected: <code>var citiesList = new[] { "Austin", "New York", "San Francisco" };

for (var eachCityIndex = 0; eachCityIndex < citiesList.Count(); eachCityIndex++)
{
    var eachCityName = citiesList[eachCityIndex];
    DoStuff();
    DoSomeOtherStuff();
}</code>
<hr></hr>
Given: <code>if (userRole == 8) // Check if Admin 
{
    
}</code>
Expected
<code>
Scanner sc=new Scanner(System.in)
string USER_ADMIN_ROLE=sc.next();
if(userAdminRole.isEqual(USER_ADMIN_ROLE)){}

</code>
<hr></code>hr>

## review6
Given: <code>public class Car
{
    public string CarMake { get; set; }
    public string CarModel { get; set; }
    public string CarColor { get; set; }

    //...
}</code>

Expected: <code>public class Car
{
    public string make { get; set; }
    public string model { get; set; }
    public string color { get; set; }

    //...
}</code>
<hr></hr>

## review 7
Given: <code>var ymdstr = DateTime.UtcNow.ToString("MMMM dd, yyyy");</code>
Expected:<code>var dateInUTC = DateTime.UtcNow.ToString("MMMM dd, yyyy");</code>
<hr></hr>

## review 9
Given: <code>public void CreateMicrobrewery(string name = null)
{
    var breweryName = !string.IsNullOrEmpty(name) ? name : "Hipster Brew Co.";
    // ...
}</code>
Expected: <code>
public void createMicrobrewery(string name= "Hipster Brew Co.")
{
    
}
</code>
