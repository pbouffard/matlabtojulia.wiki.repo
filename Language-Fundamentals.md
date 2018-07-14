# Language Fundamentals

This page maps MATLAB functionality documented in the [Language Fundamentals](https://www.mathworks.com/help/matlab/language-fundamentals.html) section of the MATLAB documentation to equivalent Julia (core language and/or package) functionality.

## Entering Commands
* [[ans]] Most recent answer
* [[clc]] Clear Command Window
* [[save]] Command Window text to file
* [[format]] Set Command Window output display format
* [[home (matlab)]] Send cursor home
* [[iskeyword]] Determine whether input is MATLAB keyword
* [[more]] Control paged output for Command Window

## Matrices and Arrays
* [[zeros]] Create array of all zeros
* [[ones]] Create array of all ones
* [[rand]] Uniformly distributed random numbers
* [[true]] Logical 1 (true)
* [[false]] Logical 0 (false)
* [[eye]] Identity matrix
* [[diag]] Create diagonal matrix or get diagonal elements of matrix
* [[blkdiag]] Construct block diagonal matrix from input arguments
* [[cat]] Concatenate arrays along specified dimension
* [[horzcat]] Concatenate arrays horizontally
* [[vertcat]] Concatenate arrays vertically
* [[repelem]] Repeat copies of array elements
* [[repmat]] Repeat copies of array
* [[linspace]] Generate linearly spaced vector
* [[logspace]] Generate logarithmically spaced vector
* [[freqspace]] Frequency spacing for frequency response
* [[meshgrid]] 2-D and 3-D grids
* [[ndgrid]] Rectangular grid in N-D space
* [[length]] Length of largest array dimension
* [[size]] Array size
* [[ndims]] Number of array dimensions
* [[numel]] Number of array elements
* [[isscalar]] Determine whether input is scalar
* [[isvector]] Determine whether input is vector
* [[ismatrix]] Determine whether input is matrix
* [[isrow]] Determine whether input is row vector
* [[iscolumn]] Determine whether input is column vector
* [[isempty]] Determine whether array is empty
* [[sort]] Sort array elements
* [[sortrows]] Sort rows of matrix or table
* [[issorted]] Determine if array is sorted
* [[issortedrows]] Determine if matrix or table rows are sorted
* [[topkrows]] Top rows in sorted order
* [[flip]] Flip order of elements
* [[fliplr]] Flip array left to right
* [[flipud]] Flip array up to down
* [[rot90]] Rotate array 90 degrees
* [[transpose]] Transpose vector or matrix
* [[ctranspose]] Complex conjugate transpose
* [[permute]] Rearrange dimensions of N-D array
* [[ipermute]] Inverse permute dimensions of N-D array
* [[circshift]] Shift array circularly
* [[shiftdim]] Shift dimensions
* [[reshape]] Reshape array
* [[squeeze]] Remove singleton dimensions
* [[colon]] Vector creation, array subscripting, and for-loop iteration
* [[end]] Terminate block of code, or indicate last array index
* [[ind2sub]] Subscripts from linear index
* [[sub2ind]] Convert subscripts to linear indices

## Operators and Elementary Operations

### Arithmetic
* [[plus]] Addition
* [[uplus]] Unary plus
* [[minus]] Subtraction
* [[uminus]] Unary minus
* [[times]] Element-wise multiplication
* [[rdivide]] Right array division
* [[ldivide]] Left array division
* [[power]] Element-wise power
* [[mtimes]] Matrix Multiplication
* [[mrdivide]] Solve systems of linear equations xA = B for x
* [[mldivide]] Solve systems of linear equations Ax = B for x
* [[mpower]] Matrix power
* [[cumprod]] Cumulative product
* [[cumsum]] Cumulative sum
* [[diff]] Differences and Approximate Derivatives
* [[movsum]] Moving sum
* [[prod]] Product of array elements
* [[sum]] Sum of array elements
* [[ceil]] Round toward positive infinity
* [[fix]] Round toward zero
* [[floor]] Round toward negative infinity
* [[idivide]] Integer division with rounding option
* [[mod]] Remainder after division (modulo operation)
* [[rem]] Remainder after division
* [[round]] Round to nearest decimal or integer
* [[bsxfun]] Apply element-wise operation to two arrays with implicit expansion enabled

### Relational Operations
* [[eq]] Determine equality
* [[ge]] Determine greater than or equal to
* [[gt]] Determine greater than
* [[le]] Determine less than or equal to
* [[lt]] Determine less than
* [[ne]] Determine inequality
* [[isequal]] Determine array equality
* [[isequaln]] Determine array equality, treating NaN values as equal

## Logical Operations

### Logical Operators: Short-circuit Logical operations with short-circuiting
* [[and]] Find logical AND
* [[not]] Find logical NOT
* [[or]] Find logical OR
* [[xor]] Find logical exclusive-OR
* [[all]] Determine if all array elements are nonzero or true
* [[any]] Determine if any array elements are nonzero
* [[false]] Logical 0 (false)
* [[find]] Find indices and values of nonzero elements
* [[islogical]] Determine if input is logical array
* [[logical]] Convert numeric values to logicals
* [[true]] Logical 1 (true)

### Set Operations
* [[intersect]] Set intersection of two arrays
* [[ismember]] Array elements that are members of set array
* [[ismembertol]] Members of set within tolerance
* [[issorted]] Determine if array is sorted
* [[setdiff]] Set difference of two arrays
* [[setxor]] Set exclusive OR of two arrays
* [[union]] Set union of two arrays
* [[unique]] Unique values in array
* [[uniquetol]] Unique values within tolerance
* [[join]] Combine two tables or timetables by rows using key variables
* [[innerjoin]] Inner join between two tables or timetables
* [[outerjoin]] Outer join between two tables or timetables

### Bit-Wise Operations
* [[bitand]] Bit-wise AND
* [[bitcmp]] Bit-wise complement
* [[bitget]] Get bit at specified position
* [[bitor]] Bit-wise OR
* [[bitset]] Set bit at specific location
* [[bitshift]] Shift bits specified number of places
* [[bitxor]] Bit-wise XOR
* [[swapbytes]] Swap byte ordering

## Data Types

### Numeric Types
* [[double]] Double-precision arrays
* [[single]] Single-precision arrays
* [[int8]] 8-bit signed integer arrays
* [[int16]] 16-bit signed integer arrays
* [[int32]] 32-bit signed integer arrays
* [[int64]] 64-bit signed integer arrays
* [[uint8]] 8-bit unsigned integer arrays
* [[uint16]] 16-bit unsigned integer arrays
* [[uint32]] 32-bit unsigned integer arrays
* [[uint64]] 64-bit unsigned integer arrays
* [[cast]] Cast variable to different data type
* [[typecast]] Convert data types without changing underlying data
* [[isinteger]] Determine if input is integer array
* [[isfloat]] Determine if input is floating-point array
* [[isnumeric]] Determine if input is numeric array
* [[isreal]] Determine whether array is real
* [[isfinite]] Array elements that are finite
* [[isinf]] Array elements that are infinite
* [[isnan]] Array elements that are NaN
* [[eps]] Floating-point relative accuracy
* [[flintmax]] Largest consecutive integer in floating-point format

### Inf Infinity
* [[intmax]] Largest value of specified integer type
* [[intmin]] Smallest value of specified integer type

### NaN Not-a-Number
* [[realmax]] Largest positive floating-point number
* [[realmin]] Smallest positive normalized floating-point number

### Characters and Strings
* [[string]] String array
* [[strings]] Create array of strings with no characters
* [[join]] Combine strings
* [[char]] Character array
* [[cellstr]] Convert to cell array of character vectors
* [[blanks]] Create character array of blanks
* [[newline]] Create newline character
* [[compose]] Convert data into formatted string array
* [[sprintf]] Format data into string
* [[strcat]] Concatenate strings horizontally
* [[convertCharsToStrings]] Convert character arrays to string arrays, leaving other arrays unaltered
* [[convertStringsToChars]] Convert string arrays to character arrays, leaving other arrays unaltered
* [[ischar]] Determine if input is character array
* [[iscellstr]] Determine if input is cell array of character vectors
* [[isstring]] Determine if input is string array
* [[isStringScalar]] Determine if input is string array with one element
* [[strlength]] Length of strings in string array
* [[isstrprop]] Determine if string is of specified category
* [[isletter]] Determine which characters are letters
* [[isspace]] Determine which characters are space characters
* [[contains]] Determine if pattern is in string
* [[count]] Count occurrences of pattern in string
* [[endsWith]] Determine if string ends with pattern
* [[startsWith]] Determine if string starts with pattern
* [[strfind]] Find one string within another
* [[sscanf]] Read formatted data from string
* [[replace]] Find and replace substrings in string array
* [[replaceBetween]] Replace substrings identified by indicators that mark their starts and ends
* [[strrep]] Find and replace substring
* [[join]] Combine strings
* [[split]] Split strings in string array
* [[splitlines]] Split string at newline characters
* [[strjoin]] Join text in array
* [[strsplit]] Split string at specified delimiter
* [[strtok]] Selected parts of string
* [[erase]] Delete substrings within strings
* [[eraseBetween]] Delete substrings between indicators that mark starts and ends of substrings
* [[extractAfter]] Extract substring after specified position
* [[extractBefore]] Extract substring before specified position
* [[extractBetween]] Extract substrings between indicators that mark starts and ends of substrings
* [[insertAfter]] Insert string after specified substring
* [[insertBefore]] Insert string before specified substring
* [[pad]] Add leading or trailing characters to strings
* [[strip]] Remove leading and trailing characters from string
* [[lower]] Convert string to lowercase
* [[upper]] Convert string to uppercase
* [[reverse]] Reverse order of characters in string
* [[deblank]] Remove trailing whitespace from end of string or character array
* [[strtrim]] Remove leading and trailing whitespace from string array or character array
* [[strjust]] Justify string or character array
* [[strcmp]] Compare strings
* [[strcmpi]] Compare strings (case insensitive)
* [[strncmp]] Compare first n characters of strings (case sensitive)
* [[strncmpi]] Compare first n characters of strings (case insensitive)
* [[regexp]] Match regular expression (case sensitive)
* [[regexpi]] Match regular expression (case insensitive)
* [[regexprep]] Replace text using regular expression
* [[regexptranslate]] Translate text into regular expression

### Dates and Time
* [[datetime]] Arrays that represent points in time

### NaT Not-a-Time
* [[years]] Duration in years
* [[days]] Duration in days
* [[hours]] Duration in hours
* [[minutes]] Duration in minutes
* [[seconds]] Duration in seconds
* [[milliseconds]] Duration in milliseconds
* [[duration]] Lengths of time in fixed-length units
* [[calyears]] Calendar duration in years
* [[calquarters]] Calendar duration in quarters
* [[calmonths]] Calendar duration in months
* [[calweeks]] Calendar duration in weeks
* [[caldays]] Calendar duration in days
* [[calendarDuration]] Lengths of time in variable-length calendar units
* [[year]] Year number
* [[quarter]] Quarter number
* [[month]] Month number and name
* [[week]] Week number
* [[day]] Day number or name
* [[hour]] Hour number
* [[minute]] Minute number
* [[second]] Second number
* [[ymd]] Year, month, and day numbers of datetime
* [[hms]] Hour, minute, and second numbers of duration
* [[split]] Split calendar duration into numeric and duration units
* [[time]] Convert time of calendar duration to duration
* [[timeofday]] Elapsed time since midnight for datetimes
* [[isdatetime]] Determine if input is datetime array
* [[isduration]] Determine if input is duration array
* [[iscalendarduration]] Determine if input is calendar duration array
* [[isnat]] Determine NaT (Not-a-Time) elements
* [[isdst]] Determine daylight saving time elements
* [[isweekend]] Determine weekend elements
* [[timezones]] List time zones
* [[tzoffset]] Time zone offset from UTC
* [[between]] Calendar math differences
* [[caldiff]] Calendar math successive differences
* [[dateshift]] Shift date or generate sequence of dates and time
* [[isbetween]] Determine elements within date and time interval
* [[datenum]] Convert date and time to serial date number
* [[datevec]] Convert date and time to vector of components
* [[exceltime]] Convert MATLAB datetime to Excel date number
* [[juliandate]] Convert MATLAB datetime to Julian date
* [[posixtime]] Convert MATLAB datetime to POSIX time
* [[yyyymmdd]] Convert MATLAB datetime to YYYYMMDD numeric value
* [[addtodate]] Modify date number by field
* [[char]] Character array
* [[string]] String array
* [[datestr]] Convert date and time to string format
* [[now]] Current date and time as serial date number
* [[clock]] Current date and time as date vector
* [[date]] Current date string
* [[calendar]] Calendar for specified month
* [[eomday]] Last day of month
* [[weekday]] Day of week
* [[etime]] Time elapsed between date vectors

### Categorical Arrays
* [[categorical]] Array that contains values assigned to categories
* [[iscategorical]] Determine whether input is categorical array
* [[discretize]] Group data into bins or categories
* [[categories]] Categories of categorical array
* [[iscategory]] Test for categorical array categories
* [[isordinal]] Determine whether input is ordinal categorical array
* [[isprotected]] Determine whether categories of categorical array are protected
* [[addcats]] Add categories to categorical array
* [[mergecats]] Merge categories in categorical array
* [[removecats]] Remove categories from categorical array
* [[renamecats]] Rename categories in categorical array
* [[reordercats]] Reorder categories in categorical array
* [[setcats]] Set categories in categorical array
* [[summary]] Print summary of table, timetable, or categorical array
* [[countcats]] Count occurrences of categorical array elements by category
* [[isundefined]] Find undefined elements in categorical array

### Tables
* [[table]] Table array with named variables that can contain different types
* [[array2table]] Convert homogeneous array to table
* [[cell2table]] Convert cell array to table
* [[struct2table]] Convert structure array to table
* [[table2array]] Convert table to homogeneous array
* [[table2cell]] Convert table to cell array
* [[table2struct]] Convert table to structure array
* [[table2timetable]] Convert table to timetable
* [[timetable2table]] Convert timetable to table
* [[readtable]] Create table from file
* [[writetable]] Write table to file
* [[detectImportOptions]] Create import options based on file content
* [[getvaropts]] Get variable import options
* [[setvaropts]] Set variable import options
* [[setvartype]] Set variable data types
* [[head]] Get top rows of table, timetable, or tall array
* [[tail]] Get bottom rows of table, timetable, or tall array
* [[summary]] Print summary of table, timetable, or categorical array
* [[height]] Number of table rows
* [[width]] Number of table variables
* [[istable]] Determine whether input is table
* [[sortrows]] Sort rows of matrix or table
* [[unique]] Unique values in array
* [[issortedrows]] Determine if matrix or table rows are sorted
* [[topkrows]] Top rows in sorted order
* [[addvars]] Add variables to table or timetable
* [[movevars]] Move variables in table or timetable
* [[removevars]] Delete variables from table or timetable
* [[splitvars]] Split multicolumn variables in table or timetable
* [[mergevars]] Combine table or timetable variables into multicolumn variable
* [[vartype]] Subscript into table or timetable by variable type
* [[rows2vars]] Reorient table or timetable so that rows become variables
* [[stack]] Stack data from multiple variables into single variable
* [[unstack]] Unstack data from single variable into multiple variables
* [[inner2outer]] Invert nested table-in-table hierarchy in tables or timetables
* [[join]] Combine two tables or timetables by rows using key variables
* [[innerjoin]] Inner join between two tables or timetables
* [[outerjoin]] Outer join between two tables or timetables
* [[union]] Set union of two arrays
* [[intersect]] Set intersection of two arrays
* [[ismember]] Array elements that are members of set array
* [[setdiff]] Set difference of two arrays
* [[setxor]] Set exclusive OR of two arrays
* [[ismissing]] Find missing values
* [[standardizeMissing]] Insert standard missing values
* [[rmmissing]] Remove missing entries
* [[fillmissing]] Fill missing values
* [[varfun]] Apply function to table or timetable variables
* [[rowfun]] Apply function to table or timetable rows
* [[findgroups]] Find groups and return group numbers
* [[splitapply]] Split data into groups and apply function
* [[groupsummary]] Group summary computations

### Timetables
* [[timetable]] Timetable array with time-stamped rows and variables of different types
* [[retime]] Resample or aggregate data in timetable, and resolve duplicate or irregular times
synchronize Synchronize timetables to common time vector, and resample or aggregate data from input * [[timetables]]
* [[lag]] Time-shift data in timetable
* [[table2timetable]] Convert table to timetable
* [[array2timetable]] Convert homogeneous array to timetable
* [[timetable2table]] Convert timetable to table
* [[istimetable]] Determine if input is timetable
* [[isregular]] Determine whether times in timetable are regular
* [[timerange]] Time range for timetable row subscripting
* [[withtol]] Time tolerance for timetable row subscripting
* [[vartype]] Subscript into table or timetable by variable type
* [[rmmissing]] Remove missing entries
* [[issorted]] Determine if array is sorted
* [[sortrows]] Sort rows of matrix or table
* [[unique]] Unique values in array

### Structures
* [[struct]] Structure array
* [[fieldnames]] Field names of structure, or public fields of COM or Java object
* [[getfield]] Field of structure array
* [[isfield]] Determine whether input is structure array field
* [[isstruct]] Determine whether input is structure array
* [[orderfields]] Order fields of structure array
* [[rmfield]] Remove fields from structure
* [[setfield]] Assign values to structure array field
* [[arrayfun]] Apply function to each element of array
* [[structfun]] Apply function to each field of scalar structure
* [[table2struct]] Convert table to structure array
* [[struct2table]] Convert structure array to table
* [[cell2struct]] Convert cell array to structure array
* [[struct2cell]] Convert structure to cell array

### Cell Arrays
* [[cell]] Cell array
* [[cell2mat]] Convert cell array to ordinary array of the underlying data type
* [[cell2struct]] Convert cell array to structure array
* [[cell2table]] Convert cell array to table
* [[celldisp]] Display cell array contents
* [[cellfun]] Apply function to each cell in cell array
* [[cellplot]] Graphically display structure of cell array
* [[cellstr]] Convert to cell array of character vectors
* [[iscell]] Determine whether input is cell array
* [[iscellstr]] Determine if input is cell array of character vectors
* [[mat2cell]] Convert array to cell array with potentially different sized cells
* [[num2cell]] Convert array to cell array with consistently sized cells
* [[strjoin]] Join text in array
* [[strsplit]] Split string at specified delimiter
* [[struct2cell]] Convert structure to cell array
* [[table2cell]] Convert table to cell array

### Function Handles
* [[feval]] Evaluate function
* [[func2str]] Construct character vector from function handle
* [[str2func]] Construct function handle from character vector
* [[localfunctions]] Function handles to all local functions in MATLAB file
* [[functions]] Information about function handle

### Map Containers
* [[containers]].Map Object that maps values to unique keys
* [[isKey]] Determine if Map object contains key
* [[keys]] Return keys of Map object
* [[remove]] Delete key-value pairs from Map object
* [[values]] Return values of Map object

### Time Series

#### Time Series Objects
* [[timeseries]] Create timeseries object
* [[addevent]] Add event to timeseries
* [[addsample]] Add data sample to timeseries object
* [[append]] Concatenate timeseries objects in time
* [[delevent]] Remove event from timeseries
* [[delsample]] Remove sample from timeseries object
* [[detrend]] Subtract mean or best-fit line from timeseries object
* [[filter]] Modify frequency content of timeseries objects
* [[idealfilter]] timeseries ideal filter
* [[plot]] Plot timeseries
* [[resample]] Resample timeseries time vector
* [[set]] Set timeseries properties
* [[setabstime]] Set timeseries times as date character vectors
* [[setinterpfunction]] Set default interpolation method for timeseries object
* [[setuniformtime]] Modify uniform timeseries time vector
* [[synchronize]] Synchronize and resample two timeseries objects using common time vector
* [[get]] Query timeseries properties
* [[getabstime]] Convert timeseries time vector to cell array
* [[getdatasamples]] Access timeseries data samples
* [[getdatasamplesize]] timeseries data sample size
* [[getinterpmethod]] timeseries interpolation method
* [[getqualitydesc]] timeseries data quality
* [[getsamples]] Subset of timeseries
* [[getsampleusingtime]] Subset of timeseries data
* [[gettsafteratevent]] Create timeseries at or after event
* [[gettsafterevent]] Create timeseries after event
* [[gettsatevent]] Create timeseries at event
* [[gettsbeforeatevent]] Create timeseries at or before event
* [[gettsbeforeevent]] Create timeseries before event
* [[gettsbetweenevents]] Create timeseries between events
* [[iqr]] Interquartile range of timeseries data
* [[max]] Maximum of timeseries data
* [[mean]] Mean of timeseries data
* [[median]] Median of timeseries data
* [[min]] Minimum of timeseries data
* [[std]] Standard deviation of timeseries data
* [[sum]] Sum of timeseries data
* [[var]] Variance of timeseries data

#### Time Series Collections
* [[tscollection]] Create tscollection object
* [[addsampletocollection]] Add sample to tscollection
* [[addts]] Add timeseries to tscollection
* [[delsamplefromcollection]] Delete sample from tscollection
* [[horzcat]] Horizontally concatenate tscollection objects
* [[removets]] Remove timeseries from tscollection
* [[resample]] Resample tscollection time vector
* [[set]] Set tscollection properties
* [[setabstime]] Set tscollection times as date character vectors
* [[settimeseriesnames]] Rename timeseries in tscollection
* [[vertcat]] Vertically concatenate tscollection objects
* [[get]] Query tscollection properties
* [[getabstime]] Convert tscollection time vector to cell array
* [[getsampleusingtime]] Subset of tscollection data
* [[gettimeseriesnames]] Names of timeseries in tscollection
* [[isempty]] Determine if tscollection is empty
* [[length]] Length of tscollection time vector
* [[size]] Size of tscollection

#### Time Series Events
* [[tsdata]].event Create tsdata.event object
* [[findEvent]] Query tsdata.event by name
* [[get]] Query tsdata.event properties
* [[getTimeStr]] Query tsdata.event times
* [[set]] Set tsdata.event properties

#### Data Type Identification
* [[iscalendarduration]] Determine if input is calendar duration array
* [[iscategorical]] Determine whether input is categorical array
* [[iscell]] Determine whether input is cell array
* [[iscellstr]] Determine if input is cell array of character vectors
* [[ischar]] Determine if input is character array
* [[isdatetime]] Determine if input is datetime array
* [[isduration]] Determine if input is duration array
* [[isenum]] Determine if variable is enumeration
* [[isfloat]] Determine if input is floating-point array
* [[isgraphics]] True for valid graphics object handles
* [[isinteger]] Determine if input is integer array
* [[isjava]] Determine if input is Java object
* [[islogical]] Determine if input is logical array
* [[isnumeric]] Determine if input is numeric array
* [[isobject]] Determine if input is MATLAB object
* [[isreal]] Determine whether array is real
* [[isstring]] Determine if input is string array
* [[isstruct]] Determine whether input is structure array
* [[istable]] Determine whether input is table
* [[istimetable]] Determine if input is timetable
* [[is]] Detect state
* [[isa]] Determine if input is object of specified class
* [[class]] Determine class of object
* [[validateattributes]] Check validity of array
* [[whos]] List variables in workspace, with sizes and types

#### Data Type Conversion
* [[char]] Character array
* [[cellstr]] Convert to cell array of character vectors
* [[int2str]] Convert integers to characters
* [[mat2str]] Convert matrix to characters
* [[num2str]] Convert numbers to character array
* [[str2double]] Convert string to double precision value
* [[str2num]] Convert character array to numeric array
* [[native2unicode]] Convert numeric bytes to Unicode character representation
* [[unicode2native]] Convert Unicode character representation to numeric bytes
* [[base2dec]] Convert text representing number in base N to decimal number
* [[bin2dec]] Convert text representation of binary number to decimal number
* [[dec2base]] Convert decimal number to character vector representing base N number
* [[dec2bin]] Convert decimal number to character vector representing binary number
* [[dec2hex]] Convert decimal number to character vector representing hexadecimal number
* [[hex2dec]] Convert text representation of hexadecimal number to decimal number
* [[hex2num]] Convert IEEE hexadecimal string to double-precision number
* [[num2hex]] Convert singles and doubles to IEEE hexadecimal strings
* [[table2array]] Convert table to homogeneous array
* [[table2cell]] Convert table to cell array
* [[table2struct]] Convert table to structure array
* [[array2table]] Convert homogeneous array to table
* [[cell2table]] Convert cell array to table
* [[struct2table]] Convert structure array to table
* [[cell2mat]] Convert cell array to ordinary array of the underlying data type
* [[cell2struct]] Convert cell array to structure array
* [[mat2cell]] Convert array to cell array with potentially different sized cells
* [[num2cell]] Convert array to cell array with consistently sized cells
* [[struct2cell]] Convert structure to cell array