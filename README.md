# Reverse__Number
    int reverse(int x) {

    long long rev=0;
    while(x!=0){
        int ld = x % 10; // gives last digit
        rev = rev *10 + ld;
        if(rev ==INT_MAX || rev > INT_MAX){// if else statements are came due to limit the constraints in rev argument, is put long long.
            return 0;
        } 
        if(rev < INT_MIN || rev == INT_MIN){
            return 0;
        }
        x =x /10;
    }
    return rev;


    
    }
};
