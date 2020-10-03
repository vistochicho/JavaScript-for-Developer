function findLongestWordLength(str) {
  //split the string and put it on a variable
  let test = str.split(" ");
  //create 2 variable with 0 value
  let oji = 0;
  let i = 0;
  //loop with one of the variable while it is smaller than the variable of the split array
  while(i < test.length){
    //if the length of the test is bigger than the other variable with value 0, update the variable with the length of the bigger length that pass the test
    if(test[i].length > oji){
      oji = test[i].length;
    }
    //increment the variable for the loop
    i++;
  }
  //return the variable that contain the biggest variable length
  return oji;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");
findLongestWordLength("Google do a barrel roll");
findLongestWordLength("What is the average airspeed velocity of an unladen swallow");
