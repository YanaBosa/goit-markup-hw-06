# goit-markup-hw-06
варіанти чекбоксів

.check-text {
  font-size: 12px;
  line-height: 1.33;
  letter-spacing: 0.04em;
  color: #757575;
  display: flex;
  align-items: center;
  position: relative;
}

.check-text::before {
  content: '';
  width: 40px;
  height: 22px;
  border: 1px solid #999999;
  border-radius: 50px;
  margin-right: 10px;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) ;

}
.check-text::after {
content: '';
  position: absolute;
left: 4px;
top: 4px;
width: 20px;
height: 20px;
background-color: rgb(110, 99, 99);
border-radius: 50px;
transition: transform 250ms cubic-bezier(0.4, 0, 0.2, 1), background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.modal-check:checked + .check-text::after {
  transform: translate(20px);
  background-color: #757575;
}
.modal-check:checked + .check-text::before {
  background-color: #854d4d;
}
варіант 2

* .check-text::before {
  content: "";
  width: 16px;
  height: 16px;
  border: 1.25px solid #2e2f42;
  border-radius: 2px;
  margin-right: 8px;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
    background-image 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.modal-check:checked + .check-text::before {
  background-color: #404bbf;
  border: none;
  background-image: url(../images/сheck-click.svg);
  background-position: center;
  background-repeat: no-repeat;
} */

/* .check-text span {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 16px;
  height: 16px;
  border: 1.25px solid #2e2f42;
  border-radius: 2px;
  margin-right: 8px;
  fill: transparent;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
    border 250ms cubic-bezier(0.4, 0, 0.2, 1),
    fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
}