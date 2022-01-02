20.
class Solution:
    def isValid(self, s: str) -> bool:
        if len(s) % 2 != 0:
            return False
        dic = {"(":")", "{":"}", "[":"]"}
        
        # stack implementation to compare two paranthesis
        stack = []
        for i in s:
            if i in dic.keys(): # means this is opening bracket
                stack.append(i)
            else:
                if stack and dic[stack[-1]] == i:
                    stack.pop()
                else:
                    return False
                
        return len(stack) == 0
                
        
 # https://leetcode.com/problems/valid-parentheses
