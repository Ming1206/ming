public static boolean isSubset(char[] firstSet, char[] sceondSet )
	{
		boolean find = false;
		
		for (int i = 0; i < sceondSet.length; i++)
		{
			for (int j = 0; j < firstSet.length; j++)
			{
				if (sceondSet[i] == firstSet[j])
				{
					find = true;
					break;
				}
			}
			if (!find) return find;
			else find = false;						
		}		
		return true;
	}
