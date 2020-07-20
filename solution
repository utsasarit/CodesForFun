import java.util.*;
public class test {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc = new Scanner(System.in);
		
		Car[] car =new Car[3];
		
		for(int i=0;i<3;i++) {
			System.out.println("enter price");
			int price=sc.nextInt(); sc.nextLine();
			System.out.println("enter model name");
			String modelName= sc.nextLine();
			System.out.println("enter model color");
			String modelColor = sc.nextLine();
			car[i] = new Car(price,modelName,modelColor);
		}
		
		System.out.println("enter price");
		int orderPrice = sc.nextInt();
		sc.close();
		
		Car[] result = carAvailable(car,orderPrice);
		
		for(int i=0; i< result.length;i++) {
			System.out.println("You may buy: \t"+result[i].getModelName()+"\t"+result[i].getModelColor());
		}
	}
	 public static Car[] carAvailable( Car[] car, int orderPrice) {
		 List<Car> list = new ArrayList<Car>();
		 
		 for(int i=0;i<3;i++) {
			 if(car[i].getPrice() < orderPrice) 
				 list.add(car[i]);
		 }
		 
		 Car[] out = new Car[list.size()];
		 out = list.toArray(out);
		 
		}
    }
