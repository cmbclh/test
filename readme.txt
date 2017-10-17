----
        hbox = QtWidgets.QHBoxLayout()
        hbox.addStretch()
        hbox.addWidget(buttonSubmit)
        hbox.addWidget(buttonLogin)

        vbox = QtWidgets.QVBoxLayout()
        vbox.addLayout(grid)
        vbox.addLayout(hbox)
        self.setLayout(vbox)

        # 连接组件信号
        buttonSubmit.clicked.connect(self.submit)
        buttonLogin.clicked.connect(self.login)