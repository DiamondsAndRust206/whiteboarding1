function noSpace(url) {

  let str = url.split(" ").join("%20");
  return str;
    
}

<!-- create a function that retruns an empty string
use a for loop to loop through the string
use and if statement to determine when a white space occurs
use slice to remove characters from white space and before
concatenate "%20"
then add the remainder of the input string back on -->

function noSpaces(input)
{
  let result = "";
  for(let i=0 ; i<input.length ; i++)
  {
    if(input[i] == ' ') {
      result = input.slice(0, input[i] + 1) + "%20" + input.slice(input[i] + 1);
    }
  }
  return result;
}

<!-- does not return the correct value -->