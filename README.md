public class bt9 {

	
	private String chuoi(String chuoi1) {
		String chuoi2 ="";
		chuoi1 = chuoi1.toLowerCase();
		String[] cat = chuoi1.split(" ");
		for (String s : cat){
			if (!s.equals(""))
				chuoi2 += String.valueOf(s.charAt(0)).toUpperCase() + s.substring(1) + " ";
		}
			chuoi2 = chuoi2.substring(0, chuoi2.length()-1);
		return chuoi2;
	}
	public static void main(String[] args) {
		System.out.println(new bt9().chuoi("khong   VAN   dat"));
	}
}
