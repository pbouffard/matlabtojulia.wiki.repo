# Language Fundamentals

This page maps MATLAB functionality documented in the [Language Fundamentals](https://www.mathworks.com/help/matlab/language-fundamentals.html) section of the MATLAB documentation to equivalent Julia (core language and/or package) functionality.

## Entering Commands
* [`ans`](ans) Most recent answer
* [`clc`](clc) Clear Command Window
* [`diary`](diary) Save Command Window text to file
* [`format`](format) Set Command Window output display format
* [`home`](home) Send cursor home
* [`iskeyword`](iskeyword) Determine whether input is MATLAB keyword
* [`more`](more) Control paged output for Command Window

## Matrices and Arrays
* [`zeros`](zeros) Create array of all zeros
* [`ones`](ones) Create array of all ones
* [`rand`](rand) Uniformly distributed random numbers
* [`true`](true) Logical 1 (true)
* [`false`](false) Logical 0 (false)
* [`eye`](eye) Identity matrix
* [`diag`](diag) Create diagonal matrix or get diagonal elements of matrix
* [`blkdiag`](blkdiag) Construct block diagonal matrix from input arguments
* [`cat`](cat) Concatenate arrays along specified dimension
* [`horzcat`](horzcat) Concatenate arrays horizontally
* [`vertcat`](vertcat) Concatenate arrays vertically
* [`repelem`](repelem) Repeat copies of array elements
* [`repmat`](repmat) Repeat copies of array
* [`linspace`](linspace) Generate linearly spaced vector
* [`logspace`](logspace) Generate logarithmically spaced vector
* [`freqspace`](freqspace) Frequency spacing for frequency response
* [`meshgrid`](meshgrid) 2-D and 3-D grids
* [`ndgrid`](ndgrid) Rectangular grid in N-D space
* [`length`](length) Length of largest array dimension
* [`size`](size) Array size
* [`ndims`](ndims) Number of array dimensions
* [`numel`](numel) Number of array elements
* [`isscalar`](isscalar) Determine whether input is scalar
* [`isvector`](isvector) Determine whether input is vector
* [`ismatrix`](ismatrix) Determine whether input is matrix
* [`isrow`](isrow) Determine whether input is row vector
* [`iscolumn`](iscolumn) Determine whether input is column vector
* [`isempty`](isempty) Determine whether array is empty
* [`sort`](sort) Sort array elements
* [`sortrows`](sortrows) Sort rows of matrix or table
* [`issorted`](issorted) Determine if array is sorted
* [`issortedrows`](issortedrows) Determine if matrix or table rows are sorted
* [`topkrows`](topkrows) Top rows in sorted order
* [`flip`](flip) Flip order of elements
* [`fliplr`](fliplr) Flip array left to right
* [`flipud`](flipud) Flip array up to down
* [`rot90`](rot90) Rotate array 90 degrees
* [`transpose`](transpose) Transpose vector or matrix
* [`ctranspose`](ctranspose) Complex conjugate transpose
* [`permute`](permute) Rearrange dimensions of N-D array
* [`ipermute`](ipermute) Inverse permute dimensions of N-D array
* [`circshift`](circshift) Shift array circularly
* [`shiftdim`](shiftdim) Shift dimensions
* [`reshape`](reshape) Reshape array
* [`squeeze`](squeeze) Remove singleton dimensions
* [`colon`](colon) Vector creation, array subscripting, and for-loop iteration
* [`end`](end) Terminate block of code, or indicate last array index
* [`ind2sub`](ind2sub) Subscripts from linear index
* [`sub2ind`](sub2ind) Convert subscripts to linear indices

## Operators and Elementary Operations

### Arithmetic
* [`plus`](plus) Addition
* [`uplus`](uplus) Unary plus
* [`minus`](minus) Subtraction
* [`uminus`](uminus) Unary minus
* [`times`](times) Element-wise multiplication
* [`rdivide`](rdivide) Right array division
* [`ldivide`](ldivide) Left array division
* [`power`](power) Element-wise power
* [`mtimes`](mtimes) Matrix Multiplication
* [`mrdivide`](mrdivide) Solve systems of linear equations xA = B for x
* [`mldivide`](mldivide) Solve systems of linear equations Ax = B for x
* [`mpower`](mpower) Matrix power
* [`cumprod`](cumprod) Cumulative product
* [`cumsum`](cumsum) Cumulative sum
* [`diff`](diff) Differences and Approximate Derivatives
* [`movsum`](movsum) Moving sum
* [`prod`](prod) Product of array elements
* [`sum`](sum) Sum of array elements
* [`ceil`](ceil) Round toward positive infinity
* [`fix`](fix) Round toward zero
* [`floor`](floor) Round toward negative infinity
* [`idivide`](idivide) Integer division with rounding option
* [`mod`](mod) Remainder after division (modulo operation)
* [`rem`](rem) Remainder after division
* [`round`](round) Round to nearest decimal or integer
* [`bsxfun`](bsxfun) Apply element-wise operation to two arrays with implicit expansion enabled

### Relational Operations
* [`eq`](eq) Determine equality
* [`ge`](ge) Determine greater than or equal to
* [`gt`](gt) Determine greater than
* [`le`](le) Determine less than or equal to
* [`lt`](lt) Determine less than
* [`ne`](ne) Determine inequality
* [`isequal`](isequal) Determine array equality
* [`isequaln`](isequaln) Determine array equality, treating NaN values as equal

## Logical Operations

### Logical Operators: Short-circuit Logical operations with short-circuiting
* [`and`](and) Find logical AND
* [`not`](not) Find logical NOT
* [`or`](or) Find logical OR
* [`xor`](xor) Find logical exclusive-OR
* [`all`](all) Determine if all array elements are nonzero or true
* [`any`](any) Determine if any array elements are nonzero
* [`false`](false) Logical 0 (false)
* [`find`](find) Find indices and values of nonzero elements
* [`islogical`](islogical) Determine if input is logical array
* [`logical`](logical) Convert numeric values to logicals
* [`true`](true) Logical 1 (true)

### Set Operations
* [`intersect`](intersect) Set intersection of two arrays
* [`ismember`](ismember) Array elements that are members of set array
* [`ismembertol`](ismembertol) Members of set within tolerance
* [`issorted`](issorted) Determine if array is sorted
* [`setdiff`](setdiff) Set difference of two arrays
* [`setxor`](setxor) Set exclusive OR of two arrays
* [`union`](union) Set union of two arrays
* [`unique`](unique) Unique values in array
* [`uniquetol`](uniquetol) Unique values within tolerance
* [`join`](join) Combine two tables or timetables by rows using key variables
* [`innerjoin`](innerjoin) Inner join between two tables or timetables
* [`outerjoin`](outerjoin) Outer join between two tables or timetables

### Bit-Wise Operations
* [`bitand`](bitand) Bit-wise AND
* [`bitcmp`](bitcmp) Bit-wise complement
* [`bitget`](bitget) Get bit at specified position
* [`bitor`](bitor) Bit-wise OR
* [`bitset`](bitset) Set bit at specific location
* [`bitshift`](bitshift) Shift bits specified number of places
* [`bitxor`](bitxor) Bit-wise XOR
* [`swapbytes`](swapbytes) Swap byte ordering

## Data Types

### Numeric Types
* [`double`](double) Double-precision arrays
* [`single`](single) Single-precision arrays
* [`int8`](int8) 8-bit signed integer arrays
* [`int16`](int16) 16-bit signed integer arrays
* [`int32`](int32) 32-bit signed integer arrays
* [`int64`](int64) 64-bit signed integer arrays
* [`uint8`](uint8) 8-bit unsigned integer arrays
* [`uint16`](uint16) 16-bit unsigned integer arrays
* [`uint32`](uint32) 32-bit unsigned integer arrays
* [`uint64`](uint64) 64-bit unsigned integer arrays
* [`cast`](cast) Cast variable to different data type
* [`typecast`](typecast) Convert data types without changing underlying data
* [`isinteger`](isinteger) Determine if input is integer array
* [`isfloat`](isfloat) Determine if input is floating-point array
* [`isnumeric`](isnumeric) Determine if input is numeric array
* [`isreal`](isreal) Determine whether array is real
* [`isfinite`](isfinite) Array elements that are finite
* [`isinf`](isinf) Array elements that are infinite
* [`isnan`](isnan) Array elements that are NaN
* [`eps`](eps) Floating-point relative accuracy
* [`flintmax`](flintmax) Largest consecutive integer in floating-point format

### Inf Infinity
* [`intmax`](intmax) Largest value of specified integer type
* [`intmin`](intmin) Smallest value of specified integer type

### NaN Not-a-Number
* [`realmax`](realmax) Largest positive floating-point number
* [`realmin`](realmin) Smallest positive normalized floating-point number

### Characters and Strings
* [`string`](string) String array
* [`strings`](strings) Create array of strings with no characters
* [`join`](join) Combine strings
* [`char`](char) Character array
* [`cellstr`](cellstr) Convert to cell array of character vectors
* [`blanks`](blanks) Create character array of blanks
* [`newline`](newline) Create newline character
* [`compose`](compose) Convert data into formatted string array
* [`sprintf`](sprintf) Format data into string
* [`strcat`](strcat) Concatenate strings horizontally
* [`convertCharsToStrings`](convertCharsToStrings) Convert character arrays to string arrays, leaving other arrays unaltered
* [`convertStringsToChars`](convertStringsToChars) Convert string arrays to character arrays, leaving other arrays unaltered
* [`ischar`](ischar) Determine if input is character array
* [`iscellstr`](iscellstr) Determine if input is cell array of character vectors
* [`isstring`](isstring) Determine if input is string array
* [`isStringScalar`](isStringScalar) Determine if input is string array with one element
* [`strlength`](strlength) Length of strings in string array
* [`isstrprop`](isstrprop) Determine if string is of specified category
* [`isletter`](isletter) Determine which characters are letters
* [`isspace`](isspace) Determine which characters are space characters
* [`contains`](contains) Determine if pattern is in string
* [`count`](count) Count occurrences of pattern in string
* [`endsWith`](endsWith) Determine if string ends with pattern
* [`startsWith`](startsWith) Determine if string starts with pattern
* [`strfind`](strfind) Find one string within another
* [`sscanf`](sscanf) Read formatted data from string
* [`replace`](replace) Find and replace substrings in string array
* [`replaceBetween`](replaceBetween) Replace substrings identified by indicators that mark their starts and ends
* [`strrep`](strrep) Find and replace substring
* [`join`](join) Combine strings
* [`split`](split) Split strings in string array
* [`splitlines`](splitlines) Split string at newline characters
* [`strjoin`](strjoin) Join text in array
* [`strsplit`](strsplit) Split string at specified delimiter
* [`strtok`](strtok) Selected parts of string
* [`erase`](erase) Delete substrings within strings
* [`eraseBetween`](eraseBetween) Delete substrings between indicators that mark starts and ends of substrings
* [`extractAfter`](extractAfter) Extract substring after specified position
* [`extractBefore`](extractBefore) Extract substring before specified position
* [`extractBetween`](extractBetween) Extract substrings between indicators that mark starts and ends of substrings
* [`insertAfter`](insertAfter) Insert string after specified substring
* [`insertBefore`](insertBefore) Insert string before specified substring
* [`pad`](pad) Add leading or trailing characters to strings
* [`strip`](strip) Remove leading and trailing characters from string
* [`lower`](lower) Convert string to lowercase
* [`upper`](upper) Convert string to uppercase
* [`reverse`](reverse) Reverse order of characters in string
* [`deblank`](deblank) Remove trailing whitespace from end of string or character array
* [`strtrim`](strtrim) Remove leading and trailing whitespace from string array or character array
* [`strjust`](strjust) Justify string or character array
* [`strcmp`](strcmp) Compare strings
* [`strcmpi`](strcmpi) Compare strings (case insensitive)
* [`strncmp`](strncmp) Compare first n characters of strings (case sensitive)
* [`strncmpi`](strncmpi) Compare first n characters of strings (case insensitive)
* [`regexp`](regexp) Match regular expression (case sensitive)
* [`regexpi`](regexpi) Match regular expression (case insensitive)
* [`regexprep`](regexprep) Replace text using regular expression
* [`regexptranslate`](regexptranslate) Translate text into regular expression

### Dates and Time
* [`datetime`](datetime) Arrays that represent points in time

### NaT Not-a-Time
* [`years`](years) Duration in years
* [`days`](days) Duration in days
* [`hours`](hours) Duration in hours
* [`minutes`](minutes) Duration in minutes
* [`seconds`](seconds) Duration in seconds
* [`milliseconds`](milliseconds) Duration in milliseconds
* [`duration`](duration) Lengths of time in fixed-length units
* [`calyears`](calyears) Calendar duration in years
* [`calquarters`](calquarters) Calendar duration in quarters
* [`calmonths`](calmonths) Calendar duration in months
* [`calweeks`](calweeks) Calendar duration in weeks
* [`caldays`](caldays) Calendar duration in days
* [`calendarDuration`](calendarDuration) Lengths of time in variable-length calendar units
* [`year`](year) Year number
* [`quarter`](quarter) Quarter number
* [`month`](month) Month number and name
* [`week`](week) Week number
* [`day`](day) Day number or name
* [`hour`](hour) Hour number
* [`minute`](minute) Minute number
* [`second`](second) Second number
* [`ymd`](ymd) Year, month, and day numbers of datetime
* [`hms`](hms) Hour, minute, and second numbers of duration
* [`split`](split) Split calendar duration into numeric and duration units
* [`time`](time) Convert time of calendar duration to duration
* [`timeofday`](timeofday) Elapsed time since midnight for datetimes
* [`isdatetime`](isdatetime) Determine if input is datetime array
* [`isduration`](isduration) Determine if input is duration array
* [`iscalendarduration`](iscalendarduration) Determine if input is calendar duration array
* [`isnat`](isnat) Determine NaT (Not-a-Time) elements
* [`isdst`](isdst) Determine daylight saving time elements
* [`isweekend`](isweekend) Determine weekend elements
* [`timezones`](timezones) List time zones
* [`tzoffset`](tzoffset) Time zone offset from UTC
* [`between`](between) Calendar math differences
* [`caldiff`](caldiff) Calendar math successive differences
* [`dateshift`](dateshift) Shift date or generate sequence of dates and time
* [`isbetween`](isbetween) Determine elements within date and time interval
* [`datenum`](datenum) Convert date and time to serial date number
* [`datevec`](datevec) Convert date and time to vector of components
* [`exceltime`](exceltime) Convert MATLAB datetime to Excel date number
* [`juliandate`](juliandate) Convert MATLAB datetime to Julian date
* [`posixtime`](posixtime) Convert MATLAB datetime to POSIX time
* [`yyyymmdd`](yyyymmdd) Convert MATLAB datetime to YYYYMMDD numeric value
* [`addtodate`](addtodate) Modify date number by field
* [`char`](char) Character array
* [`string`](string) String array
* [`datestr`](datestr) Convert date and time to string format
* [`now`](now) Current date and time as serial date number
* [`clock`](clock) Current date and time as date vector
* [`date`](date) Current date string
* [`calendar`](calendar) Calendar for specified month
* [`eomday`](eomday) Last day of month
* [`weekday`](weekday) Day of week
* [`etime`](etime) Time elapsed between date vectors

### Categorical Arrays
* [`categorical`](categorical) Array that contains values assigned to categories
* [`iscategorical`](iscategorical) Determine whether input is categorical array
* [`discretize`](discretize) Group data into bins or categories
* [`categories`](categories) Categories of categorical array
* [`iscategory`](iscategory) Test for categorical array categories
* [`isordinal`](isordinal) Determine whether input is ordinal categorical array
* [`isprotected`](isprotected) Determine whether categories of categorical array are protected
* [`addcats`](addcats) Add categories to categorical array
* [`mergecats`](mergecats) Merge categories in categorical array
* [`removecats`](removecats) Remove categories from categorical array
* [`renamecats`](renamecats) Rename categories in categorical array
* [`reordercats`](reordercats) Reorder categories in categorical array
* [`setcats`](setcats) Set categories in categorical array
* [`summary`](summary) Print summary of table, timetable, or categorical array
* [`countcats`](countcats) Count occurrences of categorical array elements by category
* [`isundefined`](isundefined) Find undefined elements in categorical array

### Tables
* [`table`](table) Table array with named variables that can contain different types
* [`array2table`](array2table) Convert homogeneous array to table
* [`cell2table`](cell2table) Convert cell array to table
* [`struct2table`](struct2table) Convert structure array to table
* [`table2array`](table2array) Convert table to homogeneous array
* [`table2cell`](table2cell) Convert table to cell array
* [`table2struct`](table2struct) Convert table to structure array
* [`table2timetable`](table2timetable) Convert table to timetable
* [`timetable2table`](timetable2table) Convert timetable to table
* [`readtable`](readtable) Create table from file
* [`writetable`](writetable) Write table to file
* [`detectImportOptions`](detectImportOptions) Create import options based on file content
* [`getvaropts`](getvaropts) Get variable import options
* [`setvaropts`](setvaropts) Set variable import options
* [`setvartype`](setvartype) Set variable data types
* [`head`](head) Get top rows of table, timetable, or tall array
* [`tail`](tail) Get bottom rows of table, timetable, or tall array
* [`summary`](summary) Print summary of table, timetable, or categorical array
* [`height`](height) Number of table rows
* [`width`](width) Number of table variables
* [`istable`](istable) Determine whether input is table
* [`sortrows`](sortrows) Sort rows of matrix or table
* [`unique`](unique) Unique values in array
* [`issortedrows`](issortedrows) Determine if matrix or table rows are sorted
* [`topkrows`](topkrows) Top rows in sorted order
* [`addvars`](addvars) Add variables to table or timetable
* [`movevars`](movevars) Move variables in table or timetable
* [`removevars`](removevars) Delete variables from table or timetable
* [`splitvars`](splitvars) Split multicolumn variables in table or timetable
* [`mergevars`](mergevars) Combine table or timetable variables into multicolumn variable
* [`vartype`](vartype) Subscript into table or timetable by variable type
* [`rows2vars`](rows2vars) Reorient table or timetable so that rows become variables
* [`stack`](stack) Stack data from multiple variables into single variable
* [`unstack`](unstack) Unstack data from single variable into multiple variables
* [`inner2outer`](inner2outer) Invert nested table-in-table hierarchy in tables or timetables
* [`join`](join) Combine two tables or timetables by rows using key variables
* [`innerjoin`](innerjoin) Inner join between two tables or timetables
* [`outerjoin`](outerjoin) Outer join between two tables or timetables
* [`union`](union) Set union of two arrays
* [`intersect`](intersect) Set intersection of two arrays
* [`ismember`](ismember) Array elements that are members of set array
* [`setdiff`](setdiff) Set difference of two arrays
* [`setxor`](setxor) Set exclusive OR of two arrays
* [`ismissing`](ismissing) Find missing values
* [`standardizeMissing`](standardizeMissing) Insert standard missing values
* [`rmmissing`](rmmissing) Remove missing entries
* [`fillmissing`](fillmissing) Fill missing values
* [`varfun`](varfun) Apply function to table or timetable variables
* [`rowfun`](rowfun) Apply function to table or timetable rows
* [`findgroups`](findgroups) Find groups and return group numbers
* [`splitapply`](splitapply) Split data into groups and apply function
* [`groupsummary`](groupsummary) Group summary computations

### Timetables
* [`timetable`](timetable) Timetable array with time-stamped rows and variables of different types
* [`retime`](retime) Resample or aggregate data in timetable, and resolve duplicate or irregular times
synchronize Synchronize timetables to common time vector, and resample or aggregate data from input * [`timetables`](timetables)
* [`lag`](lag) Time-shift data in timetable
* [`table2timetable`](table2timetable) Convert table to timetable
* [`array2timetable`](array2timetable) Convert homogeneous array to timetable
* [`timetable2table`](timetable2table) Convert timetable to table
* [`istimetable`](istimetable) Determine if input is timetable
* [`isregular`](isregular) Determine whether times in timetable are regular
* [`timerange`](timerange) Time range for timetable row subscripting
* [`withtol`](withtol) Time tolerance for timetable row subscripting
* [`vartype`](vartype) Subscript into table or timetable by variable type
* [`rmmissing`](rmmissing) Remove missing entries
* [`issorted`](issorted) Determine if array is sorted
* [`sortrows`](sortrows) Sort rows of matrix or table
* [`unique`](unique) Unique values in array

### Structures
* [`struct`](struct) Structure array
* [`fieldnames`](fieldnames) Field names of structure, or public fields of COM or Java object
* [`getfield`](getfield) Field of structure array
* [`isfield`](isfield) Determine whether input is structure array field
* [`isstruct`](isstruct) Determine whether input is structure array
* [`orderfields`](orderfields) Order fields of structure array
* [`rmfield`](rmfield) Remove fields from structure
* [`setfield`](setfield) Assign values to structure array field
* [`arrayfun`](arrayfun) Apply function to each element of array
* [`structfun`](structfun) Apply function to each field of scalar structure
* [`table2struct`](table2struct) Convert table to structure array
* [`struct2table`](struct2table) Convert structure array to table
* [`cell2struct`](cell2struct) Convert cell array to structure array
* [`struct2cell`](struct2cell) Convert structure to cell array

### Cell Arrays
* [`cell`](cell) Cell array
* [`cell2mat`](cell2mat) Convert cell array to ordinary array of the underlying data type
* [`cell2struct`](cell2struct) Convert cell array to structure array
* [`cell2table`](cell2table) Convert cell array to table
* [`celldisp`](celldisp) Display cell array contents
* [`cellfun`](cellfun) Apply function to each cell in cell array
* [`cellplot`](cellplot) Graphically display structure of cell array
* [`cellstr`](cellstr) Convert to cell array of character vectors
* [`iscell`](iscell) Determine whether input is cell array
* [`iscellstr`](iscellstr) Determine if input is cell array of character vectors
* [`mat2cell`](mat2cell) Convert array to cell array with potentially different sized cells
* [`num2cell`](num2cell) Convert array to cell array with consistently sized cells
* [`strjoin`](strjoin) Join text in array
* [`strsplit`](strsplit) Split string at specified delimiter
* [`struct2cell`](struct2cell) Convert structure to cell array
* [`table2cell`](table2cell) Convert table to cell array

### Function Handles
* [`feval`](feval) Evaluate function
* [`func2str`](func2str) Construct character vector from function handle
* [`str2func`](str2func) Construct function handle from character vector
* [`localfunctions`](localfunctions) Function handles to all local functions in MATLAB file
* [`functions`](functions) Information about function handle

### Map Containers
* [`containers`](containers).Map Object that maps values to unique keys
* [`isKey`](isKey) Determine if Map object contains key
* [`keys`](keys) Return keys of Map object
* [`remove`](remove) Delete key-value pairs from Map object
* [`values`](values) Return values of Map object

### Time Series

#### Time Series Objects
* [`timeseries`](timeseries) Create timeseries object
* [`addevent`](addevent) Add event to timeseries
* [`addsample`](addsample) Add data sample to timeseries object
* [`append`](append) Concatenate timeseries objects in time
* [`delevent`](delevent) Remove event from timeseries
* [`delsample`](delsample) Remove sample from timeseries object
* [`detrend`](detrend) Subtract mean or best-fit line from timeseries object
* [`filter`](filter) Modify frequency content of timeseries objects
* [`idealfilter`](idealfilter) timeseries ideal filter
* [`plot`](plot) Plot timeseries
* [`resample`](resample) Resample timeseries time vector
* [`set`](set) Set timeseries properties
* [`setabstime`](setabstime) Set timeseries times as date character vectors
* [`setinterpfunction`](setinterpfunction) Set default interpolation method for timeseries object
* [`setuniformtime`](setuniformtime) Modify uniform timeseries time vector
* [`synchronize`](synchronize) Synchronize and resample two timeseries objects using common time vector
* [`get`](get) Query timeseries properties
* [`getabstime`](getabstime) Convert timeseries time vector to cell array
* [`getdatasamples`](getdatasamples) Access timeseries data samples
* [`getdatasamplesize`](getdatasamplesize) timeseries data sample size
* [`getinterpmethod`](getinterpmethod) timeseries interpolation method
* [`getqualitydesc`](getqualitydesc) timeseries data quality
* [`getsamples`](getsamples) Subset of timeseries
* [`getsampleusingtime`](getsampleusingtime) Subset of timeseries data
* [`gettsafteratevent`](gettsafteratevent) Create timeseries at or after event
* [`gettsafterevent`](gettsafterevent) Create timeseries after event
* [`gettsatevent`](gettsatevent) Create timeseries at event
* [`gettsbeforeatevent`](gettsbeforeatevent) Create timeseries at or before event
* [`gettsbeforeevent`](gettsbeforeevent) Create timeseries before event
* [`gettsbetweenevents`](gettsbetweenevents) Create timeseries between events
* [`iqr`](iqr) Interquartile range of timeseries data
* [`max`](max) Maximum of timeseries data
* [`mean`](mean) Mean of timeseries data
* [`median`](median) Median of timeseries data
* [`min`](min) Minimum of timeseries data
* [`std`](std) Standard deviation of timeseries data
* [`sum`](sum) Sum of timeseries data
* [`var`](var) Variance of timeseries data

#### Time Series Collections
* [`tscollection`](tscollection) Create tscollection object
* [`addsampletocollection`](addsampletocollection) Add sample to tscollection
* [`addts`](addts) Add timeseries to tscollection
* [`delsamplefromcollection`](delsamplefromcollection) Delete sample from tscollection
* [`horzcat`](horzcat) Horizontally concatenate tscollection objects
* [`removets`](removets) Remove timeseries from tscollection
* [`resample`](resample) Resample tscollection time vector
* [`set`](set) Set tscollection properties
* [`setabstime`](setabstime) Set tscollection times as date character vectors
* [`settimeseriesnames`](settimeseriesnames) Rename timeseries in tscollection
* [`vertcat`](vertcat) Vertically concatenate tscollection objects
* [`get`](get) Query tscollection properties
* [`getabstime`](getabstime) Convert tscollection time vector to cell array
* [`getsampleusingtime`](getsampleusingtime) Subset of tscollection data
* [`gettimeseriesnames`](gettimeseriesnames) Names of timeseries in tscollection
* [`isempty`](isempty) Determine if tscollection is empty
* [`length`](length) Length of tscollection time vector
* [`size`](size) Size of tscollection

#### Time Series Events
* [`tsdata`](tsdata).event Create tsdata.event object
* [`findEvent`](findEvent) Query tsdata.event by name
* [`get`](get) Query tsdata.event properties
* [`getTimeStr`](getTimeStr) Query tsdata.event times
* [`set`](set) Set tsdata.event properties

#### Data Type Identification
* [`iscalendarduration`](iscalendarduration) Determine if input is calendar duration array
* [`iscategorical`](iscategorical) Determine whether input is categorical array
* [`iscell`](iscell) Determine whether input is cell array
* [`iscellstr`](iscellstr) Determine if input is cell array of character vectors
* [`ischar`](ischar) Determine if input is character array
* [`isdatetime`](isdatetime) Determine if input is datetime array
* [`isduration`](isduration) Determine if input is duration array
* [`isenum`](isenum) Determine if variable is enumeration
* [`isfloat`](isfloat) Determine if input is floating-point array
* [`isgraphics`](isgraphics) True for valid graphics object handles
* [`isinteger`](isinteger) Determine if input is integer array
* [`isjava`](isjava) Determine if input is Java object
* [`islogical`](islogical) Determine if input is logical array
* [`isnumeric`](isnumeric) Determine if input is numeric array
* [`isobject`](isobject) Determine if input is MATLAB object
* [`isreal`](isreal) Determine whether array is real
* [`isstring`](isstring) Determine if input is string array
* [`isstruct`](isstruct) Determine whether input is structure array
* [`istable`](istable) Determine whether input is table
* [`istimetable`](istimetable) Determine if input is timetable
* [`is*`](is) Detect state
* [`isa`](isa) Determine if input is object of specified class
* [`class`](class) Determine class of object
* [`validateattributes`](validateattributes) Check validity of array
* [`whos`](whos) List variables in workspace, with sizes and types

#### Data Type Conversion
* [`char`](char) Character array
* [`cellstr`](cellstr) Convert to cell array of character vectors
* [`int2str`](int2str) Convert integers to characters
* [`mat2str`](mat2str) Convert matrix to characters
* [`num2str`](num2str) Convert numbers to character array
* [`str2double`](str2double) Convert string to double precision value
* [`str2num`](str2num) Convert character array to numeric array
* [`native2unicode`](native2unicode) Convert numeric bytes to Unicode character representation
* [`unicode2native`](unicode2native) Convert Unicode character representation to numeric bytes
* [`base2dec`](base2dec) Convert text representing number in base N to decimal number
* [`bin2dec`](bin2dec) Convert text representation of binary number to decimal number
* [`dec2base`](dec2base) Convert decimal number to character vector representing base N number
* [`dec2bin`](dec2bin) Convert decimal number to character vector representing binary number
* [`dec2hex`](dec2hex) Convert decimal number to character vector representing hexadecimal number
* [`hex2dec`](hex2dec) Convert text representation of hexadecimal number to decimal number
* [`hex2num`](hex2num) Convert IEEE hexadecimal string to double-precision number
* [`num2hex`](num2hex) Convert singles and doubles to IEEE hexadecimal strings
* [`table2array`](table2array) Convert table to homogeneous array
* [`table2cell`](table2cell) Convert table to cell array
* [`table2struct`](table2struct) Convert table to structure array
* [`array2table`](array2table) Convert homogeneous array to table
* [`cell2table`](cell2table) Convert cell array to table
* [`struct2table`](struct2table) Convert structure array to table
* [`cell2mat`](cell2mat) Convert cell array to ordinary array of the underlying data type
* [`cell2struct`](cell2struct) Convert cell array to structure array
* [`mat2cell`](mat2cell) Convert array to cell array with potentially different sized cells
* [`num2cell`](num2cell) Convert array to cell array with consistently sized cells
* [`struct2cell`](struct2cell) Convert structure to cell array