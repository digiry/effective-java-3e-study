# 아이템13. clone 재정의는 주의해서 진행하라

clone 규약

필수

x.clone() != x 반드시 true

x.clone().getClass() == x.getClass() , true

충분

x.clone().equals(x) , true