```
//求三个班级的平均分，每班四个人，用户自己输入分数
public class classAve{

	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		int classNum = 3;
		int stuNum = 4;
		double ave = 0;		
		double sum = 0;
		
		for(int i = 1; i <= classNum ; i++)
		{
			System.out.println("***请输入第"+i+"个班级的成绩***"); 
			for(int j = 1; j <= stuNum; j++)
			{	

				System.out.print("请输入第"+j+"名学生的成绩："); 
				double score = input.nextDouble();
				sum += score;
			}	
			ave = sum/stuNum;
			System.out.println("第"+i+"个班学生成绩平均分为："+ave);
			sum = 0;//**记得清空总分，不然会累积到下一个班级总分。导致平均分变化。**
		}
	}
}
```
