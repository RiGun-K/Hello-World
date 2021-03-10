# Hello-World
First My Project
public class Television {
	
	int channel; // 채널
	int voulume; // 볼륨
	boolean onOff; // 전원
	void print() {				// print 메소드는 Television 클래스 안에 포함됨  , 메소드 몸체이며 channel,volume 은 멤버연산자(.)필요없음
		System.out.println("채널은"+ channel + "이고 볼륨은 "+ voulume + "입니다"); //print에 입력된 각 객체들을 출력
	}
	
	int getChannel() {
		return channel;}         // main 메소드 이전에  설정  getChannel의 변수에 channel 값을 반환  == 26,27열
	
	// 3개의 필드 생성 , 자료형 + 변수이름; 
	// 클래스 정의는 단순히 객체를 찍어내기 위한 틀임 , 실제 객체가 아님 ! 클래스는 객체가 아니다
	public static void main(String[] args) {   // public 과 main 메소드 작성, main이 있어야 실행, main메소드와 tv클래스와는 상관없음,
		// TODO Auto-generated method stub	   // tv클래스 안에 main이 들어있을 뿐임.
		
		Television mytv = new Television(); // Television 의 클래스를 이용해서 객체를 생성한다. = new 연산자 
		mytv.channel = 5;					  // 각 객체의 해당하는 값을 입력
		mytv.voulume = 7;
		mytv.onOff   = true;
		mytv.print();			// mytv의 객체에 선언된 값을 print에 담아옴  ,, mytv (객체 참조변수) print (메소드이름)
		
		int ch = mytv.getChannel();					// 선언된 getChannel에 int형 'ch'라는 변수에 mytv에 해당하는 값을 저장
		System.out.println("현재 나의 채널은" + ch +"입니다.");		
		
		
		Television yourtv = new Television();	// mytv 와 yourtv는 별개의 객체이다.
		yourtv.channel = 3;
		yourtv.voulume = 11;
		yourtv.onOff = true;
		yourtv.print();
/*		
		System.out.println("내 텔레비전의 채널은 " + mytv.channel + "이고 볼륨은 " + mytv.voulume + "이고 전원상태는 " + mytv.onOff + "입니다.");
	
		System.out.println("당신의 텔레비전의 채널은" + yourtv.channel + "이고 볼륨은 " + yourtv.voulume + "이고 전원상태는 " + yourtv.onOff + "입니다.");
	}	
	
		Television tv1 = new Television(); // tv1이라는 참조변수
		Television tv2 = tv1; // 참조변수를 복사하면 동일한 객체를 참조 = tv2에 tv1을 대입하면 tv1의 값이 tv2로 복사됨
*/
		
//		tv1 = null;    		  // 객체를 가리키는 참조변수 tv1은 하나도 남아있지 않음 , 객체 제거
	
	// A tv = new A();     / tv = 참조변수 선언 ( tv 클래스의 객체를 참조)
	//					   / new A(); = tv 클래스의 객체를 생성 , 객체의 참조값을 반환   ,,  = = 생성된 새 객체의 참조값(주소)를 참조 변수 tv에 저장
	// tv.channel = 7;   <-- tv가 참조하는 객체로부터 channel이라는 필드(객체 상태)에 접근하여 7을 저장한다.
	
	//기초 변수 - int double 같은 기초 자료형의 값을 실제 저장,
	//참조 변수 - 객체를 참조할떄 사용되는 변수로써 참조값(주소값)이 저장.
	
//	int x = 10, y = 20;
//	y = x;		등호의 오른쪽 x의 값이 y로 대입된다. 
	
	// p211 메소드 3/7
}
}
