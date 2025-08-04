class ModelNameAG(AgGrid):
    selection_configs = {
        # 1. 모든 선택지가 다 나옴 (자동 수집)
        "column_name": {
            "type": "radio"
        },

        # 2. 별도로 커스텀된 선택지를 명시한 경우 커스텀된 선택지가 나옴
        "column_name": {
            "column_name": "radio",
            "labels": ["테스트", "테스트2"]
        }

        # 3. 기본값 {} -> 기본값을 모든 선택지로 하지 않은 이유는 type이 명시되어야하고 값이 너무 많을 수 있기 때문에
    }