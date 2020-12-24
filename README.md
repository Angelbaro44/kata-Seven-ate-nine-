# kata-Seven-ate-nine-
Description:
Seven is a hungry number and its favourite food is number 9. Whenever it spots 9 through the hoops of 8, it eats it! Well, not anymore, because you are going to help the 9 by locating that particular sequence (7,8,9) in an array of digits and tell 7 to come after 9 instead. Seven "ate" nine, no more! (If 9 is not in danger, just return the same array)



Test Cases:
-
    Test.describe("Tests", function(){

    Test.assertSimilar(hungrySeven([7,8,9]), [8,9,7]);
    Test.assertSimilar(hungrySeven([7,7,7,8,9]),[8,9,7,7,7]);
    Test.assertSimilar(hungrySeven([8,7,8,9,8,9,7,8]),[8,8,9,8,9,7,7,8]);
    Test.assertSimilar(hungrySeven([8,7,8,7,9,8]),[8,7,8,7,9,8]);
    });

    Test.describe("Random tests", function(){

    function Check(arr){
     var str = arr.join("");
      while(/789/.test(str)){
      str=str.replace(/789/,"897");
      }
      return str.split('').map(Number);
    }

    for(var i=0;i<50;i++){
    var r1 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r2 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r3 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r4 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r5 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r6 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r7 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r8 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r9 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r10 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r11 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r12 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r13 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r14 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r15 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r16 = (Math.floor(Math.random()*(10 - 7) + 7));
    var r17 = 7;
    var r18 = 8;
    var r19 = 9;
    var r20 = (Math.floor(Math.random()*(10 - 7) + 7));

    console.log(r1,r2,r3,r4,r5,r6,r7,r8,r9,r10, r11,r12,r13,r14,r15,r16,r17,r18,r19,r20);
    Test.assertSimilar(hungrySeven([r1,r2,r3,r4,r5,r6,r7,r8,r9,r10, r11,r12,r13,r14,r15,r16,r17,r18,r19,r20]),Check([r1,r2,r3,r4,r5,r6,r7,r8,r9,r10, r11,r12,r13,r14,r15,r16,r17,r18,r19,r20]));
    }
    });
