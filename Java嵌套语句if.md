```
package com.kone

public class HelloKK {
    public static void main(String[] args) {
		int score = 80;
		String sex = "女";
        if(score>80)
        {
            if(sex.equals("女")){
                System.out.println("进入女子组决赛");
            }
            else{
                System.out.println("进入男子组决赛");
            }
        }
        else
        {
            System.out.println("未进入决赛");    
        }
	}
}
```
