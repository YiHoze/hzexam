# hzexam

hzexam.sty는 시험지 또는 문제집을 만들기 위한 레이텍 패키지이다.
주요 매크로는 다음과 같다.


    \QAsetup{
        file=undefined, 
        counter=1, 
        overwrite=true, 
        zeros=3, 
        teacher=true,   
        answer-sheet=true,
        question-no=1
    }

    \begin{premise}*[숫자]
    지문 또는 문제
    \end{premise}

    \qa{문제}[보기| 보기; ...]{객관식 또는 단답형 정답}
    \qa|{문제}[보기| 보기; ...]{서술형 정답}
    \qa*{하위 문제}[보기| 보기; ...]{서술형 정답}
    \ca{숫자}
    \ca*{단답}
    
    \begin{QAwrite}
    \end{QAwrite}

    \QAinput{.../...}{숫자, 숫자-숫자, 숫자}
    \QAinput{.../...}{*}

    \InputAnswerSheet
