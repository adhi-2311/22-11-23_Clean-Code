## review1.cs
Given : <code>int d</code>
<br></br>
Expected: <code>int elapsedTimeInDays</code>
<hr></hr>

## review2.cs
Given : <code>var dataFromDb = db.GetFromService().ToList(); // Get List of employees </code>
<br></br>
Expected: <code>var employeeList = employeeService.GetEmployeeList().ToList(); // Get List of employees </code>

<hr></hr>

## review3.cs
Given : 
<code>
int iCounter;
string strFullName;
DateTime dModifiedDate;</code>
<br></br>
Expected: 
<code>
int counter;
string fullName;
DateTime modifiedDate;
</code>

## review4.cs
Given : 
<code>
public bool IsShopOpen(string pDay, int pAmount)
{
    // some logic
}
</code>
<br></br>
Expected: 
<code>
public bool IsShopOpen(string day, int amount)
{
    // some logic
}
</code>

## review5.cs
Given : 
<code>
const int DAYS_IN_WEEK = 7;
const int daysInMonth = 30;

var songs = new List<string> { 'Back In Black', 'Stairway to Heaven', 'Hey Jude' };
var Artists = new List<string> { 'ACDC', 'Led Zeppelin', 'The Beatles' };

bool EraseDatabase() {}
bool Restore_database() {}

class animal {}
class Alpaca {}
</code>
<br></br>
Expected: 
<code>
const int daysInWeek = 7;
const int daysInMonth = 30;

var songs = new List<string> { 'Back In Black', 'Stairway to Heaven', 'Hey Jude' };
var artists = new List<string> { 'ACDC', 'Led Zeppelin', 'The Beatles' };

bool eraseDatabase() {}
bool restoreDatabase() {}

class animal {}
class alpaca {}
</code>

## review6.cs
Given : 
<code>
public class Employee
{
    public Datetime sWorkDate { get; set; } // get set Start Working Date
    public Datetime modTime { get; set; } // get set Modification Time
}
</code>
<br></br>
Expected: 
<code>
public class Employee
{
    public Datetime startingWorkDate { get; set; } // get set Start Working Date
    public Datetime modifiedTime { get; set; } // get set Modification Time
}
</code>

## review7.cs
Given : 
<code>
var employeephone;

public double CalculateSalary(int workingdays, int workinghours)
{
    // some logic
}
</code>
<br></br>
Expected: 
<code>
var employeePhone;

public double calculateSalary(int workingDays, int workingHours)
{
    // some logic
}
</code>

