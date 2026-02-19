# QA-DSA--9--palindrome


var isPalindrome = function(x) {
    if(x<0){
        return false
    }
    let copyofx=x
    let rev=0
    while(x>0){
        let rem = x %10
        rev=(10*rev)+rem
        x=Math.floor(x/10)
    }
    return rev == copyofx
};
