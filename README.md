body {
  line-height: 1.6;
  color: #333;
}

header {
  background: url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e') no-repeat center center/cover;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: white;
  position: relative;
}

header::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
}

header .content {
  z-index: 2;
}

header h1 {
  font-size: 3rem;
}

header p {
  font-size: 1.2rem;
  margin: 1rem 0;
}

.btn {
  padding: 0.8rem 1.5rem;
  background: #f76c6c;
  color: white;
  border: none;
  cursor: pointer;
  font-size: 1rem;
  transition: background 0.3s ease;
}

.btn:hover {
  background: #ff4c4c;
}

section.features {
  padding: 4rem 2rem;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  background-color: #f9f9f9;
}

.feature {
  background: white;
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  text-align: center;
}

.feature h3 {
  margin-bottom: 1rem;
}

footer {
  background: #333;
  color: white;
  text-align: center;
  padding: 1.5rem 1rem;
}