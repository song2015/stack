# stackpackage stack;

import java.util.ArrayList;

public class arrayListStack {

		public static void main(String[] args) {
			Sta s = new Sta();
	        
	        s.push("a");
	        s.push("b");
	        s.push("c");
	        System.out.println(s.peek());
	        System.out.println(s.pop());
		}
	}

class Sta1{
		ArrayList<String> list=new ArrayList<>();
		
		public void push(String x)
		{
	        list.add(x);
	    }
		
		private int m=list.size()-1;
		
		public String pop()
		{
			if(!list.isEmpty())
			{
				return ((ArrayList<String>) list).remove(m);
	        }
			else return null; 
		}
		public String peek()
		{
			if(!list.isEmpty())
			{
	        return ((ArrayList<String>) list).get(m);
	        }
			else return null; 
		}
		public boolean isEmpty()
		{
	        return list.isEmpty();
	    }
    }
