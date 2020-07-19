class Solution {
public:
    string addBinary(string a, string b) {
        int m = a.length()-1;
        int n = b.length()-1;
        int carry = 0;
        int sum = 0;
        string result = "";
        while(m>=0 || n>=0) {
            sum = carry;
            if(m >= 0) {
                sum += a[m]-'0';
                m--;
            }
            if(n >= 0) {
                sum += b[n]-'0';
                n--;
            }
            carry = (sum>1)?1:0;
            if(sum%2 == 0)
                result += "0";
            else
                result += "1";
        }
        if(carry)
            result += to_string(carry);
        reverse(result.begin(), result.end());
        return result;
    }
};
