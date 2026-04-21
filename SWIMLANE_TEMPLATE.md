{
  "metadata": {
    "flowName": "프로세스명 (예: 추출된 핵심 흐름 이름)",
    "category": "Swimlane",
    "version": "v1.0.0",
    "updatedAt": "생성일시 (ISO 8601 형식)",
    "actors": [
      "AI가 코드/문맥에서 추출한 동적 주체 1 (예: 게스트 유저)",
      "동적 주체 2 (예: 결제 마이크로서비스)",
      "동적 주체 3 (예: 사내 ERP 시스템)"
    ]
  },
  "architecture": {
    "diagramType": "flowchart",
    "mermaidCode": "flowchart TD\n  subgraph Actor1 [게스트 유저]\n    A1_1([시작 노드])\n    A1_2[일반 액션 노드]\n  end\n\n  subgraph Actor2 [결제 마이크로서비스]\n    A2_1{조건 분기 노드}\n  end\n\n  subgraph Actor3 [사내 ERP 시스템]\n    A3_1[(데이터베이스 노드)]\n    A3_2([종료 노드])\n  end\n\n  A1_1 --> A1_2\n  A1_2 --> A2_1\n  A2_1 -- 조건 A --> A3_1\n  A2_1 -- 조건 B --> A3_2\n  A3_1 --> A3_2"
  }
}
